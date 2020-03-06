/* eslint-disable vue/valid-template-root */
<style>
.overlap
{
    max-width: 150px;
    max-height: 150px;
    overflow: hidden;
    padding:10px
}
</style>
<style>
#page-wraps {
   
    width: 100%;
  
    position: relative;
    

}

#lefts {
    
    width: 50%;
    height: auto;
   
    float: left;
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
  
}

#customers td, #customers th {
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

    <div class="vx-card p-6" style="" >
     <!--UPDATE START-->
      <table width="100%" border="0" class="tables">
         <tr>
           
            <td width="10%">   
            </td>
            <td width="50%"><center><h1><font color="#7367f0">TDS Form 26<br></font></h1></center></td>
            <td width="20%"  align="right">
       
          </td>
          </tr>
</table>
<br>
<table width="100%" border="0" class="tables"  align="center">
<tr>
    <td></td>
<td class="overlap"  width="33%" id="div.example"> 
    <vs-radio class="w-full" v-align="right"  size="small" v-model="radio1" vs-value="luis">Purchase Voucher</vs-radio>
</td>
<td class="overlap"   width="33%"> 
    <vs-radio class="w-full"  size="small" v-model="radio1" vs-value="luis">TDS Voucher</vs-radio>
</td>
<td class="overlap"   width="33%"> 
    <vs-radio class="w-full"  size="small" v-model="radio1" vs-value="luis">All</vs-radio>
</td>
</tr>
</table>
<br>
<table width="100%" border="0" class="tables"  align="center">
<tr>
        <td id="overlap">Type</td>
        <td class="overlap"> 
            <select class="w-full selectp">
                <option value=""></option>
            </select>
        </td>
</tr>

<tr>
        <td id="overlap">
            Issue Date 
            </td>
        <td id="overlap">
            <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
        </td>
        <td width="30%" id="overlap" align="right">
            TDS@
        </td>
        <td id="overlap">
            <vs-input  class="w-full"  size="small" v-model="input1"/>
        </td>
        <td></td>
    </tr><br>
    <tr>
        <td id="overlap" >
            BSR Code
        </td>
        <td id="overlap">
            <vs-input class="w-full" size="small" v-model="input1" />
        </td>
    </tr><br>
    <tr>
        <td id="overlap">
            Bank Name
        </td>
        <td id="overlap">
            <vs-input class="w-full" size="small" v-model="input1" />
        </td>
    </tr><br>
    <tr>
        <td id="overlap">
            Period From
        </td>
        <td id="overlap">
            <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
        </td>
        <td width="30%" id="overlap" align="right">
            To
        </td>
        <td id="overlap">
            <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
        </td>
    </tr>
</table><br>
<br>
<table width="100%" border="0" class="tables"  >
    <tr>
    <td></td>
        <td class="overlap"  width="33%"> 
            <vs-radio class="w-full" v-align="right"  size="small" v-model="radio1" vs-value="luis">Purchase Voucher</vs-radio>
        </td>
        <td class="overlap"   width="33%"> 
            <vs-radio class="w-full"  size="small" v-model="radio1" vs-value="luis">TDS Voucher</vs-radio>
        </td>
        <td class="overlap"   width="33%"> 
            <vs-radio class="w-full"  size="small" v-model="radio1" vs-value="luis">All</vs-radio>
        </td>
    </tr>
</table>
       <div align="right" style="padding-top: 5px">
        <br>

      <div class="mid" align="">
        <br>
        <br>&nbsp;&nbsp;&nbsp;&nbsp;
                <center><vs-button  color="primary" type="filled">Edit</vs-button>&nbsp;
                <vs-button  color="primary" type="filled" style="!">Export</vs-button>&nbsp;
                <vs-button  color="primary" type="filled" style="!">Print</vs-button>&nbsp;
                 <vs-button  color="primary" type="filled" style="!">Deposit</vs-button>&nbsp;
                </center>
        

      </div>
      </div>

</div>
</template>






