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
</style>

     <!--Mini CSS used , {{now}}, {{currentday}} variable is used to get current date-->

<template>

    <div class="vx-card p-6" style="" >
     <!--UPDATE START-->
      <table width="100%" border="0" class="tables">
     <tr>
      <td width="25%">  
      </td>
       <td width="50%"><center><h1 class="text-primary">Trial Balance<br/><h4><font color="grey">View</font></h4></h1></center></td>
       <td width="25%"  align="right">Today {{now}}<br/> {{currentday}}            
        </td>
      </tr>
        <br/>
      </table>  
       
      <table border="0" width="100%" >   
          <td width="30%">
      <div class="vx-row mb-3">
        <div class="vx-col sm:w-1/6 " >
          <span> Period From </span>
        </div>
            <!--Used for date picking -->
        <div class="vx-col sm:w-1/6 w-full">
           <flat-pickr  v-model="date" size="small" style="width:180px; height:25px;"  placeholder="choose Date" />
        </div>
      </div>
            <div class="vx-row mb-3">
        <div class="vx-col sm:w-1/6 " >
          <span> Upto </span>
        </div>
            <!--Used for date picking -->
        <div class="vx-col sm:w-1/6 w-full">
           <flat-pickr  v-model="date" size="small" style="width:180px; height:25px;"  placeholder="choose Date" />
        </div>
      </div>
      </td>
      <td width="40%">
          </td>
      <td width="30%">
          <div class="vx-row mb-3">
        <div class="vx-col sm:w-1/6 " >
          <span>Selected Debit</span>
        </div>
        <div class="vx-col sm:w-1/5">
           <vs-input v-model="vno" size="small" style="width:180px; height:24px;" placeholder="" />
        </div>
      </div>
      <div class="vx-row mb-3">
        <div class="vx-col sm:w-1/6 " >
          <span>Credit</span>
        </div>
        <div class="vx-col sm:w-1/5">
           <vs-input v-model="vno" size="small" style="width:180px; height:24px;" placeholder="" />
        </div>
      </div>
          </td>
      </table>

      
      

<div align="right" >
        <br>
      <div class="right" align="right">
        <br>
        &nbsp;
         <vs-button class="mr-3 mb-2" style= "width:80px" size="small">Options</vs-button>
        &nbsp;
         <vs-button class="mr-3 mb-2" style= "width:80px" size="small">Export</vs-button>
      </div>
    </div> 
    <br/>     


   <!--Table start here -->
<div  style="overflow-x:auto;">  
<table id="customers" >
  <tr >
    <th class="bg-primary">Account Name</th>
    <th class="bg-primary">City Name</th>
    <th class="bg-primary">Qtc</th>
    <th class="bg-primary">Debit</th>
    <th class="bg-primary">Credit</th>
     <th class="bg-primary">delete</th>
  </tr>
      <!--cashvouchars is a variables use for FOR LOOP, Vue.js function are used to perform action like add/delete row and sow notifications -->
      <!--Any Numeric Input validation and input will show right hand (dir="rtl"),(@keypress="onlyNumber") use for int val-->

<tr v-for="(cashVaucher, k) in cashVauchers" :key="k">  
    <td scope="row">
        <vs-input class="w-full" size="small" v-model="cashVaucher.accountname" v-on:keyup.enter="addNewRowEnterkey(k,cashVaucher)" />
    </td>
    <td>
      <vs-input class="w-full" size="small"  v-model="cashVaucher.cityname" v-on:keyup.enter="addNewRowEnterkey(k,cashVaucher)" />
    </td>
    <td>
      <vs-input class="w-full"  size="small" v-model="cashVaucher.Qtc" @change="totaladd(cashVaucher)" dir="rtl"  @keypress="onlyNumber" v-on:keyup.enter="addNewRowEnterkey(k,cashVaucher)"/>
    </td>
    <td><vs-input class="w-full" size="small" v-model="cashVaucher.debitt" v-on:keyup.enter="addNewRowEnterkey(k,cashVaucher)"/></td>
    <td><vs-input class="w-full" size="small" v-model="cashVaucher.credit" @change="totaladd(cashVaucher)" dir="rtl" @keypress="onlyNumber" v-on:keyup.enter="addNewRowEnterkey(k,cashVaucher)"/></td>
     <td align="center"><vs-button size="small" icon-pack="feather" icon="icon-trash" color="danger" style="margin:3px;"  @click="deleteRow(k, cashVaucher)"></vs-button></td>
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
    </div> <i class="far fa-trash-alt" @click="deleteRow(k, cashVaucher)"></i>
<br/>
    <div style="overflow-x:auto;"  width="100%">  
      <table  border="0" width="100%">
        <tr>
          <td class="hiden" width="0%"></td>
          <td  width="10%">Search:</td>
         <td width="20%"><vs-input class="w-full" size="small" v-model="input1" /></td>
          <td class="hiden" width="15%"></td>
          <td>
            <vs-input class="w-full" size="small"  v-model="totalcount" />
          </td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr> 
      </table>
    </div>
    <div align="right" style="padding-top: 10px">
       
      <div class="right" align="right">
        <table>
            <td>
         <vs-button class="button"  style= "width:80px" size="small" @click="print">Print</vs-button>
            </td>
             &nbsp; 
            <td>
         <vs-button class="button"  style= "width:80px" size="small" @click="submit">Submit</vs-button>
         </td>
          &nbsp; 
        <td>
         <vs-button class="mr-3 mb-2" style= "width:80px" size="small">Exit</vs-button>
        </td>
        </table>
      </div>
    </div>   
    &nbsp;   
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
            cashVauchers: [{
            accountname: '',
            cityname: '',
            qty: '',
            debit: '',
            credit: ''
            }]
        } 
    },
    components:{
      flatPickr
    },
    methods:{
          addNewRow(){
              this.cashVauchers.push({
                accountname: '',
            cityname: '',
            qty: '',
            debit: '',
            credit: ''
            });
          },
         addNewRowEnterkey(index, cashVaucher) {
               var idx = this.cashVauchers.indexOf(cashVaucher);
                 var len = this.cashVauchers.length;
            console.log(idx,index);
            if (len-1==index) {
                this.cashVauchers.push({
                accountname: '',
            cityname: '',
            qty: '',
            debit: '',
            credit: ''
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
        deleteRow(index, cashVaucher) {
            var idx = this.cashVauchers.indexOf(cashVaucher);
            console.log(idx, index);
            if (idx > -1) {
                this.cashVauchers.splice(idx, 1);
            }
            this.deleteNotify();
        },
        pop(){
           this.cashVauchers.pop({
                accountname: '',
            cityname: '',
            qty: '',
            debit: '',
            credit: ''
            });
            this.deleteNotify();
        },
         saveInvoice() {
            alert(JSON.stringify(this.cashVauchers));
        },
        totaladd(cashVaucher){
             var total = parseFloat(cashVaucher.payment) * parseFloat(cashVaucher.discount);
           this.totalcount=total;
            this.calculateTotal(); 
        },  
          deletec(){
              this.cashVauchers.pop({
               accountname: '',
            cityname: '',
            qty: '',
            debit: '',
            credit: ''
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