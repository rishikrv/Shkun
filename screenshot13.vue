<style>
.overlap
{
    
    max-width: 150px;
    max-height: 150px;
    overflow: hidden;
   
}
</style>
<style>
#page-wraps {
   
    width: 100%;
    position: relative;
    
}
#center {
    
    width: 100%;
    height: auto;
   
    float: center;
    padding-right: 9%;
   
    
    
}
#rights {
    width: 50%;
    height: auto;
    float: left;
   
    padding-left: 9%;
  
}
</style>
<style>
#page-wrap {
   
    width: 100%;
    margin: 40px auto;
    position: relative;
    
}
#left {
    
    width: 33%;
    height: auto;
   
    float: left;
    padding-right: 8%;
    
    
}
#mid {
    width: 33%;
    height: auto;
    float: left;
   
    padding-left: 8%;
  
}
#rightt {
    
    width: 34%;
    height: auto;
    float: left;
    padding-right: 2.5%;
    padding-left: 2.5%;
}
</style>
<style>
.selectp
{
  border-color: #7367f0;
  background-color:White;
}
.btn {
  background-color: #7367f0;
  border: none;
  color: white;
  padding: 12px 16px;
  font-size: 16px;
  
  cursor: pointer;
  border-radius: 12px;
}
/* Darker background on mouse-over */
.btn:hover {
  background-color: RoyalBlue;
}
</style>

<style>
#customers {
  font-family: "Trebuchet MS", Arial, Helvetica, sans-serif;
  border-collapse: collapse;
  width: 100%;
  
  width: 100%;  
}
#customers td, #customers th {
  border: 1px solid #ddd;
  
 #customers th {
  border: 1px solid #ddd; 
}
#customers tr:nth-child(even){background-color: #f2f2f2;}
#customers tr:hover {background-color: #ddd;}
#customers th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;
  background-color: #7367f0;
  color: white;
}
</style>
<style>
.right {
  position: static;
  right: 0px;
  
  padding: 10px;
  
   width: 100%;
   min-width: 10px;  
   max-width: 300px;
}
</style>

<style type="text/css">
@media screen and (min-width: 601px) {
  div.example {
    font-size: 15px;
    background-color:white; 
    padding: 55px;
    
    border-color: #7367f0;
     border-top-style: solid;
     border-bottom-style: solid;
  }
}
@media screen and (max-width: 600px) {
  div.example {
    font-size: 10px;
    background-color:white; 
    padding: 10px;
    
    border-color: #7367f0;
    border-top-style: solid;
    border-bottom-style: solid;
  }
  
}
.btns {
   width: 100%;
   min-width: 10px;  
   max-width: 300px; 
}
</style>
<style type="text/css">
  #middlecol {
   
    width: 100%;
    
  
  }
 
  .tables 
{
    table-layout:fixed;
    width:100%;
    
    
}
.users {
  table-layout: fixed;
  white-space: nowrap;
}
.users td {
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
/* Column widths are based on these cells */
.rowid {
  width: 4%;
  
   
}
</style>
<template>
@@ -224,268 +21,252 @@
     <!--UPDATE START-->
      <table width="100%" border="0" class="tables">
     <tr>
      <td width="25%">

      <td width="25%">  
      </td>
       <td width="50%"><center><h1>Bank Voucher<br><h4><font color="blue">View</font></h4></h1></center></td>
       <td width="25%"  align="right">Design Chq.    Today 28-02-2020 <br> Fridday      
       <td width="50%"><center><h1 class="text-primary">Bank Voucher<br/><h4><font color="grey">View</font></h4></h1></center></td>
       <td width="25%"  align="right">Today {{now}}<br/> {{currentday}}            
        </td>
      </tr>



      </table>


        <br/>
      </table>         
    <!--UPDATE END-->

    <table border="0" width="100%" class="tables">
        <tr>
            <td width="80%" align="left">
                <table border="0" class="tables" align="left">
                <tr>
                <td class="overlap">
                  Voucher Dt
                </td>
                <td class="overlap"> 
                 <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
                </td>

                </tr>
                <tr>
                  <td>

                <div class="overlap">
                    <span><p>Voucher.No</p></span>
                </div>
                </td>
                <td>

                     <vs-input class="w-full" size="small" v-model="input1" />

                </td>


                </tr>
                </table>


            </td>


            <td width="10%"></td>
      <td width="50%"  align="right">


              <div align="right">

     <div class="vx-row mb-3">
        <div class="vx-col sm:w-1/6 " >
          <span >  Voucher Dt </span>
        </div>
            </td>
        </tr>

    </table>

<br>

	<table border="0" width="100%" class="tables">
        <tr>
            <td width="80%" align="left">
                <table border="0" class="tables" align="left">

                <tr>
                  <td>

                <div class="overlap">
                    <span><p>Bank Name</p></span>
                </div>
                </td>
                <td>

                     <vs-input class="w-full" size="small" v-model="input1" />

                </td>


                </tr>
                </table>


            </td>


            <td width="10%"></td>
      <td width="50%"  align="right">


              <div align="right">

            <!--Used for date picking -->
        <div class="vx-col sm:w-1/6 w-full">
           <flat-pickr  v-model="date" size="small" style="width:175px; height:25px;"  placeholder="choose Date" />
        </div>
            </td>
        </tr>

    </table>



<br>
<div style="overflow-x:auto;">  
<table id="customers">
  <tr>
    <th>Account Name</th>
    <th>Payment</th>
    <th>Receipt</th>
    <th>Discount</th>
    <th>Total</th>
    <th>Bnk.Chg.</th>
    <th>Chq.No.Bank</th>
    <th>Remarks</th>
  </tr>
  <tr>

    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>

  </tr>
  <tr>
      </div>
        <div class="vx-row mb-3">
        <div class="vx-col sm:w-1/6 " >
          <span>Voucher No</span>
        </div>
        <div class="vx-col sm:w-1/5">
        <vs-input class="w-full" size="small" v-model="Vouchno"  />    
            </div>
      </div>
      <div class="vx-row mb-3">
        <div class="vx-col sm:w-1/6 " >
          <span>Bank Name</span>
        </div>
        <div class="vx-col sm:w-1/5">
           <vs-input class="w-full"  v-model="bank" size="small" />
        </div>
      </div>
<br/>

    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>

  </tr>
  <tr>

    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>

  </tr>
  <tr>

    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>

<div  style="overflow-x:auto;">  
<table id="customers" >
  <tr >
    <th class="bg-primary">Account Name</th>
    <th class="bg-primary">Payment</th>
    <th class="bg-primary">Receipt</th>
    <th class="bg-primary">Discount</th>
    <th class="bg-primary">Total</th>
     <th class="bg-primary">Bnk.Chg</th>
     <th class="bg-primary">Chq.No.Bank</th>
    <th class="bg-primary">Remarks</th>
    <th class="bg-primary">Delete</th>
  </tr>
  <tr>

    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>

  <tr v-for="(bankVoucher, k) in bankVouchers" :key="k">  
    <td scope="row">
        <vs-input class="w-full" size="small" v-model="bankVoucher.accountname" v-on:keyup.enter="addNewRowEnterkey(k,bankVoucher)" />
    </td>
    <td>
      <vs-input class="w-full" size="small"  v-model="bankVoucher.payment" @change="totaladd(bankVoucher)"  @keypress="onlyNumber" v-on:keyup.enter="addNewRowEnterkey(k,bankVoucher)" />
    </td>
    <td>
      <vs-input class="w-full"  size="small" v-model="bankVoucher.receipt" @change="totaladd(bankVoucher)" dir="rtl"   v-on:keyup.enter="addNewRowEnterkey(k,bankVoucher)"/>
    </td>
    <td><vs-input class="w-full" size="small" v-model="bankVouchers.discount"  @change="totaladd(bankVoucher)" @keypress="onlyNumber" v-on:keyup.enter="addNewRowEnterkey(k,bankVoucher)"/></td>
    <td><vs-input class="w-full" size="small" v-model="bankVoucher.total" @change="totaladd(bankVoucher)" dir="rtl" @keypress="onlyNumber" v-on:keyup.enter="addNewRowEnterkey(k,bankVoucher)"/></td>
    <td><vs-input class="w-full" size="small" v-model="bankVoucher.bnkchq"  dir="rtl" @keypress="onlyNumber" v-on:keyup.enter="addNewRowEnterkey(k,bankVoucher)"/></td>
    <td><vs-input class="w-full" size="small" v-model="bankVoucher.chqno" dir="rtl" @keypress="onlyNumber" v-on:keyup.enter="addNewRowEnterkey(k,bankVoucher)"/></td>
    <td><vs-input class="w-full" size="small" v-model="bankVoucher.remarks"  dir="rtl" @keypress="onlyNumber" v-on:keyup.enter="addNewRowEnterkey(k,bankVoucher)"/></td>
     <td align="center"><vs-button size="small" icon-pack="feather" icon="icon-trash" color="danger" style="margin:3px;"  @click="deleteRow(k, bankVoucher)"></vs-button></td>
  </tr>
  <tr>

    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>

  </tr>

</table>



    </div>

      <div id="example">
        <!--IMPORT THE SCRIPT FOR ADDING ROWS AND USE THIS BUTTON-->
      <!--<button v-on:click="add_row">Add Row</button>-->

      <button class="btn"><i class="fa fa-plus"></i></button>

    </div> 




    <div>
    <div align="center">

    <table border="0"   cellspacing="5" class="tables" >
      <tr>

        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
         <td><vs-input class="w-full" size="small" v-model="input1" /></td>
      </tr>


    </table>
    </div>

    </div>





      <!--
      <table width="100%">
      <tr>
        <td width="80%"></td>
        <td width="10%">
      
        <vs-button  color="primary" type="filled">Print</vs-button>
        
      </td>
      <td  width="10%">
        <vs-button  color="primary" type="filled" style="!">Submit</vs-button>
      </td>
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
    </div> <i class="far fa-trash-alt" @click="deleteRow(k, bankVoucher)"></i>
<br/>
<div style="overflow-x:auto;"  width="100%">  
      <table  border="0" width="100%">
        <tr>
          <td class="hiden" width="13%"></td>
          <td><vs-input class="w-full" size="small" v-model="totalcount" /></td>
          <td><vs-input class="w-full" size="small" v-model="input1" dir="rtl" @keypress="onlyNumber" /> </td>
          <td><vs-input class="w-full" size="small" v-model="input2" dir="rtl" @keypress="onlyNumber" /></td>
          <td><vs-input class="w-full" size="small" v-model="input3" dir="rtl" @keypress="onlyNumber" /></td>
        </tr> 
      </table>
      -->
      <div align="right" style="padding-top: ">
    </div>
<div align="right" style="padding-top: 10px">
        <br>

      <div class="right" align="right">
        <br>
        <vs-button  color="primary" type="filled">Print</vs-button>
         <vs-button class="button"  @click="print">Print</vs-button>
        &nbsp;
        <vs-button  color="primary" type="filled" style="!">Submit</vs-button>

         <vs-button class="button"  @click="submit">Submit</vs-button>

      </div>
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
            Vouchno:'',
            bank:'',
            input1:'',
            input2:'',
            input3:'',
            input4:'',
            bankVouchers: [{
            accountname: '',
            payment: '',
            receipt: '',
            discount: '',
            total: '',
            bnkchq: '',
            chqno: '',
            remarks: ''
            }]
        } 
    },
    components:{
      flatPickr
    },
    methods:{
          addNewRow(){
              this.bankVouchers.push({
              accountname: '',
              payment: '',
              receipt: '',
              discount: '',
              total: '',
              bnkchq: '',
              chqno: '',
              remarks: ''
            });
          },
         addNewRowEnterkey(index, bankVoucher) {
               var idx = this.bankVouchers.indexOf(bankVoucher);
                 var len = this.bankVouchers.length;
            console.log(idx,index);
            if (len-1==index) {
                this.bankVouchers.push({
                accountname: '',
                payment: '',
                receipt: '',
                discount: '',
                total: '',
                bnkchq: '',
                chqno: '',
                remarks: ''
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
        deleteRow(index, bankVoucher) {
            var idx = this.bankVouchers.indexOf(bankVoucher);
            console.log(idx, index);
            if (idx > -1) {
                this.bankVouchers.splice(idx, 1);
            }
            this.deleteNotify();
        },
        pop(){
           this.bankVouchers.pop({         
              accountname: '',
              payment: '',
              receipt: '',
              discount: '',
              total: '',
              bnkchq: '',
              chqno: '',
              remarks: ''
            });
            this.deleteNotify();
        },
         saveInvoice() {
            alert(JSON.stringify(this.bankVouchers));
        },
        totaladd(bankVoucher){
             var total = parseFloat(bankVoucher.payment) * parseFloat(bankVoucher.discount);
           this.totalcount=total;
            this.calculateTotal(); 
        },  
          deletec(){
              this.bankVouchers.pop({       
              accountname: '',
              payment: '',
              receipt: '',
              discount: '',
              total: '',
              bnkchq: '',
              chqno: '',
              remarks: ''
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
