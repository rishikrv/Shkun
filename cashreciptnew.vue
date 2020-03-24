<style>
#customers {
  font-family: "Trebuchet MS", Arial, Helvetica, sans-serif;
  border-collapse: collapse;
  width: 100%; 
}
 #customers th {
  border: 1px solid #ddd;
}
#customers th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;
  background-color: #7367f0;
  color: white;
}
 .tables 
{
    table-layout:fixed;
    width:100%;
    padding-left: 36%;
}
</style>


<template>

    <div class="vx-card p-6" style="" >
     <!--UPDATE START-->
      <table width="100%" border="0" >
     <tr>
      <td width="25%">
        
      </td>
       <td width="50%"><center><h1>Cash Receipt<br/><h4><font color="blue">View</font></h4></h1></center></td>
       <td width="25%"  align="right">Today {{now}}<br/> {{currentday}}            
        </td>
      </tr>
        <br/>
      </table>      
    <!--UPDATE END-->
      <div class="vx-row mb-3">
        <div class="vx-col sm:w-1/6 " >
          <span> Voucher Dt </span>
        </div>
        <div class="vx-col sm:w-1/6 w-full">
           <flat-pickr  v-model="date" size="small" style="width:180px; height:25px;"  placeholder="choose Date" />
        </div>
      </div>
      <div class="vx-row mb-3">
        <div class="vx-col sm:w-1/6 " >
          <span>Voucher No</span>
        </div>
        <div class="vx-col sm:w-1/5">
           <vs-input v-model="date" size="small" style="width:180px; height:24px;" placeholder="" />
        </div>
      </div>
  
<br/>
<table width="100%" border="0" >
    <td width="50%">
      <table border="0">
          <td width="34%">
              Bank Name
          </td>
           <td ><vs-input class="w-full" size="small" v-model="input1" /></td>
           <td width="30%"><vs-input class="w-full" size="small" v-model="input1" /></td>
          </table>
        
    </td>

    <td width="50%"  class="tables">
            <vs-checkbox v-model="checkBox1">Bank Option</vs-checkbox>     
    </td>

</table>	
<br/>
<div  style="overflow-x:auto;"  width="100%" >  
<table id="customers">
  <tr >
    <th class="bg-primary">Account Name</th>
    <th class="bg-primary">City Name</th>
    <th class="bg-primary">Narration</th>
    <th class="bg-primary">Receipt No.</th>
    <th class="bg-primary">Payment</th>
    <th class="bg-primary">Receipt</th>
    <th class="bg-primary">Disount</th>
    <th class="bg-primary">delete</th>
  </tr>
<tr v-for="(cashReceipt, k) in cashReceipts" :key="k">  
    <td scope="row"><vs-input class="w-full" size="small" v-model="cashReceipt.accountno" v-on:keyup.enter="addNewRow" /></td>
    <td><vs-input class="w-full" size="small"  v-model="cashReceipt.cityname"  /></td>
    <td><vs-input class="w-full" size="small"  v-model="cashReceipt.narration"  /></td>
    <td><vs-input class="w-full"  size="small" v-model="cashReceipt.receiptno"   @keypress="onlyNumber"/></td>
    <td><vs-input class="w-full"  size="small" v-model="cashReceipt.payment" @change="totaladd(cashReceipt)" dir="rtl"  @keypress="onlyNumber"/></td>
    <td><vs-input class="w-full" size="small" v-model="cashReceipt.receipt" /></td>
    <td><vs-input class="w-full" size="small" v-model="cashReceipt.discount" @change="totaladd(cashReceipt)" dir="rtl" @keypress="onlyNumber"  v-on:keyup.enter="addNewRow"/></td>
    <td align="center"><vs-button type="border" size="small" icon-pack="feather" icon-no-border icon="icon-trash" color="danger" style="margin:3px;"  @click="deleteRow(k, cashReceipt)"></vs-button></td>
  </tr>
  </table>
</div>
  <br/>
    <div id="example">
      <vs-button class="button" size="small" @click="addNewRow"><i class="fa fa-plus"></i></vs-button>
     &nbsp;
      <vs-button class="button" size="small"  @click="pop"><i class="fa fa-minus"></i></vs-button>
          &nbsp;
        <vs-button class="button" size="small" @click="saveInvoice">show all data</vs-button>
    </div> <i class="far fa-trash-alt" @click="deleteRow(k, cashReceipt)"></i>
<br/>
    <div style="overflow-x:auto;"  width="100%">  
      <table  border="0" width="100%">
        <tr>
          <td class="hiden" width="13%"></td>
          <td  width="13%">Cash in hand:</td>
          <td width="8%" align="right" ><b class="text-primary">₹</b> 0.00 </td>
          <td class="hiden" width="6%"></td>
          <td>
                <vs-input class="w-full" size="small"  v-model="totalcount" />
       
          </td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr> 
      </table>
    </div>
    <div align="right" style="padding-top: 10px">
        <br>
      <div class="right" align="right">
        <br>
         <vs-button class="button"  @click="print">Print</vs-button>
        &nbsp;
         <vs-button class="button"  @click="submit">Submit</vs-button>

      </div>
    </div>      
  </div>
</template>


<script>
import  flatPickr  from 'vue-flatpickr-component';
import  'flatpickr/dist/flatpickr.css';
export default {
  data() {
        return {
            date:null,
            totalcount:0,
            cashReceipts: [{
            accountno: '',
            cityname: '',
            narration: '',
            receiptno:'',
            payment: '',
            receipt: '',
            discount: ''
            }]
        } 
    },
    components:{
      flatPickr
    },
    methods:{
        addNewRow() {
            this.cashReceipts.push({
                accountno: '',
                cityname: '',
                narration: '',
                receiptno:'',
                payment: '',
                receipt: '',
                discount: ''
            });
        },
        deleteRow(index, cashReceipt) {
            var idx = this.cashReceipts.indexOf(cashReceipt);
            console.log(idx, index);
            if (idx > -1) {
                this.cashReceipts.splice(idx, 1);
            }
        },
        pop(){
           this.cashReceipts.pop({
                accountno: '',
                cityname: '',
                narration: '',
                receiptno:'',
                payment: '',
                receipt: '',
                discount: ''
            });
        },
         saveInvoice() {
            alert(JSON.stringify(this.cashReceipts));
        },
        totaladd(cashReceipt){
             var total = parseFloat(cashReceipt.payment) * parseFloat(cashReceipt.discount);
           this.totalcount=total;
            this.calculateTotal(); 
        },
        
          deletec(){
              this.cashReceipts.pop({
                accountno: '',
                cityname: '',
                narration: '',
                receiptno:'',
                payment: 0,
                receipt: '',
                discount: 0
            });
          },
         onlyNumber($event) {
             
                let keyCode = ($event.keyCode ? $event.keyCode : $event.which);
                if ((keyCode < 48 || keyCode > 57) && keyCode !== 46) { // 46 is dot
                  return   $event.preventDefault();
                }
                else return null;          
          }
    },
    created() {
      for(var i=0;i<4;i++){
         this.addNewRow();
      }
    },
    computed: {
        now: function () {  
          var today = new Date();
          var date = today.getFullYear()+'-'+(today.getMonth()+1)+'-'+today.getDate();
          return date;
        },
        currentday: function(){
           var today = new Date();
           var weekday=['Sunday','Monday','Tuesday','Wednesday','Thursday','Friday','Saturday'];
            var  currenday = weekday[today.getDay()];
            return currenday;
        }
    }
}
</script>

