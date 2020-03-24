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

     <!--Mini CSS used , {{now}}, {{currentday}} variable is used to get current date-->

<template>

    <div class="vx-card p-6" style="" >
     <!--UPDATE START-->
      <table width="100%" border="0" >
     <tr>
      <td width="25%">  
      </td>
       <td width="50%"><center><h1 class="text-primary">Cash Receipt<br/><h4><font color="grey">View</font></h4></h1></center></td>
       <td width="25%"  align="right">Today {{now}}<br/> {{currentday}}            
        </td>
      </tr>
        <br/>
      </table>      
      <div class="vx-row mb-3">
        <div class="vx-col sm:w-1/6 " >
          <span> Voucher Dt </span>
        </div>
            <!--Used for date picking -->
        <div class="vx-col sm:w-1/6 w-full">
           <flat-pickr  v-model="date" size="small" style="width:150px; height:24px;"  placeholder="choose Date" />
        </div>
      </div>
      <div class="vx-row mb-3">
        <div class="vx-col sm:w-1/6 " >
          <span>Voucher No</span>
        </div>
        <div class="vx-col sm:w-1/5">
           <vs-input v-model="vno" size="small" style="width:150px; height:24px;" placeholder="" />
        </div>
      </div>
<br/>
<table width="100%" border="0" >
    <td width="50%">
      <table border="0" >
          <td width="35%">
              Bank Name
          </td>
           <td ><vs-input v-model="vno" size="small" style="width:150px; height:24px;" placeholder="" /></td>
           <td><vs-input v-model="vno" size="small" style="width:150px; height:24px;" placeholder="" /></td>
          </table>
        
    </td>

    <td width="50%"  class="tables">
            <vs-checkbox v-model="checkBox1">Bank Option</vs-checkbox>     
    </td>

</table>	
<br/>
   <!--Table start here -->
<div  style="overflow-x:auto;">  
<table id="customers" >
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
      <!--cashvouchars is a variables use for FOR LOOP, Vue.js function are used to perform action like add/delete row and sow notifications -->
      <!--Any Numeric Input validation and input will show right hand (dir="rtl"),(@keypress="onlyNumber") use for int val-->

<tr v-for="(cashReceipt, k) in cashReceipts" :key="k">  
    <td scope="row">
        <vs-input class="w-full" size="small" v-model="cashReceipt.accountno" v-on:keyup.enter="addNewRowEnterkey(k,cashReceipt)" />
    </td>
     <td><vs-input class="w-full" size="small"  v-model="cashReceipt.cityname"  /></td>
    <td>
      <vs-input class="w-full" size="small"  v-model="cashReceipt.narration" v-on:keyup.enter="addNewRowEnterkey(k,cashReceipt)" />
    </td>
    <td><vs-input class="w-full"  size="small" v-model="cashReceipt.receiptno"   @keypress="onlyNumber"/></td>
    <td>
      <vs-input class="w-full"  size="small" v-model="cashReceipt.payment" @change="totaladd(cashReceipt)" dir="rtl"  @keypress="onlyNumber" v-on:keyup.enter="addNewRowEnterkey(k,cashReceipt)"/>
    </td>
    <td><vs-input class="w-full" size="small" v-model="cashReceipt.receipt" v-on:keyup.enter="addNewRowEnterkey(k,cashReceipt)"/></td>
    <td><vs-input class="w-full" size="small" v-model="cashReceipt.discount" @change="totaladd(cashReceipt)" dir="rtl" @keypress="onlyNumber" v-on:keyup.enter="addNewRowEnterkey(k,cashReceipt)"/></td>
     <td align="center"><vs-button size="small" icon-pack="feather" icon="icon-trash" color="danger" style="margin:3px;"  @click="deleteRow(k, cashReceipt)"></vs-button></td>
  </tr>
  </table>
</div>
  <br/>
    <div id="example">
      <vs-button class="button" size="small" @click="addNewRow();addNotify()" ><i class="fa fa-plus"></i></vs-button>
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

 <!--Script Start here all the action like @click and all method written above are define in this script, please useunique key value -->

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
          addNewRow(){
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
         addNewRowEnterkey(index,cashReceipt) {
               var idx = this.cashReceipts.indexOf(cashReceipt);
                 var len = this.cashReceipts.length;
            console.log(idx,index);
            if (len-1==index) {
                this.cashReceipts.push({
                accountno: '',
                cityname: '',
                narration: '',
                receiptno:'',
                payment: '',
                receipt: '',
                discount: ''
                });
                     this.addNotify();
            }
        },
        deleteNotify(){
            this.$vs.notify({
              text: 'Row is deleted',
              color: "danger",
              iconPack: 'feather',
              icon:'icon-trash'
             })
      },
       addNotify(){
            this.$vs.notify({
              text: 'Row is Added',
              color: "primary",
              iconPack: 'feather',
              icon:'icon-plus'
             })
      },
        deleteRow(index, cashReceipt) {
            var idx = this.cashReceipts.indexOf(cashReceipt);
            console.log(idx, index);
            if (idx > -1) {
                this.cashReceipts.splice(idx, 1);
            }
            this.deleteNotify();
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
            this.deleteNotify();
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
                payment: '',
                receipt: '',
                discount: ''
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