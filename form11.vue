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
    
    width: 10%;
    height: auto;
   
    float: left;
    padding-right: 8%;
    
    
}

#mid {
    width: 45%;
    height: auto;
    float: left;
   
    padding-left: 8%;
  
}

#rightt {
    
    width: 45%;
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
        <td width="33%">
        </td>
        <td width="33%"><center><h1>Purchase Summary Party</h1></center></td>
        <td width="33%"></td>
    </tr>
    </table>
<br>

<div id="page-wrap" class="div.example">
    <div id="left">
      <table border="0" width="100%" cellspacing="5" class="tables">
        <tr>
          <td class="overlap"></td>
          <td></td>
        </tr>
        <tr>
          <td class="overlap"></td>
          <td></td>
        </tr>
        <tr>
          <td class="overlap"></td>
          <td></td>
        </tr>
      </table>
    </div>
    <div id="rightt" class="div.example">
      <table border="0" width="100%" cellspacing="5" class="tables" >
        <tr>
            <td id="overlap" class=""  >
                <vs-radio class="w-full" width="50%"  size="small" v-model="radio1" vs-value="luis">Total Summary</vs-radio>
            </td>
        </tr>
        <tr>
            <td><vs-radio class="w-full"  size="small" v-model="radio1" vs-value="luis">Month Wise</vs-radio></td>
            <td class="overlap">
            <vs-checkbox  color="primary" v-model="checkbox"><font color="#7367f0">B2B</font></vs-checkbox>&nbsp;
        </td> 
        </tr>
        <tr>
            <td><vs-radio class="w-full"  size="small" v-model="radio1" vs-value="luis">Date Wise</vs-radio></td>
            <td class="overlap">
            <vs-checkbox  color="primary" v-model="checkbox"><font color="#7367f0">Less Dr/Cr Note</font></vs-checkbox>&nbsp;
        </td> 
        </tr>
        <tr>
            <td><vs-radio class="w-full"  size="" v-model="radio1" vs-value="luis">Certificate</vs-radio></td>
        </tr>
      </table>
    </div>	
        <div id="mid"  class="div.example">
          <table border="0" width="100%" cellspacing="5" class="tables">
        <tr>
           <td id="overlap"  class="div.example" width="50%" align="center">Upto</td>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
           <td id="overlap" class="div.example" align="center">Maximum Qty</td>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
           <td id="overlap" class="div.example" align="center">Minimum Value</td>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
           <td id="overlap" class="div.example" align="center">Maximum Value</td>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
      </table>
        </div>       
		<div style="clear:both;"></div>
	</div>
<table border="0" width="100%" cellspacing="5" class="div.example">
    <tr>
        <td id="overlap" align="center" class="div.example">
                <center><vs-button  color="primary" type="filled">Select Ledger Accounts</vs-button>&nbsp;
                <vs-button  color="primary" type="filled" style="!">Select Stock Items</vs-button>&nbsp;
                </center></td>
    </tr>
</table>
    
<div id="page-wrap"  class="div.example">
    <div id="left"  class="div.example">
      <table border="0" width="100%" cellspacing="5" class="tables">
        <tr>
          <td class="overlap"></td>
          <td></td>
        </tr>
        <tr>
          <td id="overlap"></td>
          <td></td>
        </tr>
        <tr>
          <td id="overlap"></td>
          <td></td>
        </tr>
        <tr>
            <td></td>
        </tr>
      </table>
    </div>
    <div id="rightt"  class="div.example">
      <table border="0" width="100%" cellspacing="5" class="tables">
        <tr>
            <td id="overlap" class="div.example" align="center">From</td>
            <td><vs-input type="date" class="w-full" size="small" v-model="date" /></td>
        </tr>
        <tr>
            <td id="overlap"  class="div.example" align="center">City Name</td>
            <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
            <td id="overlap"  class="div.example" align="center">Agent</td>
            <td ><vs-input class="w-full" size="small" v-model="input1" /></td>

        </tr>
        <tr>
            <td id="overlap"  class="div.example" align="center">Full Address</td>
            <td id="overlap" class="div.example">
            <select class="w-full selectp">
                <option value="">Yes</option>
                <option value="">No</option>
            </select>
        </td>    
           
        </tr>
        <tr>
        <td id="overlap"  class="div.example" align="center">Product Comp.</td>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
      </tr>
      </table>
    </div>
    <div id="mid"  class="div.example">
          <table border="0" width="100%" cellspacing="5"  class="tables">
        <tr>
           <td id="overlap"  class="div.example" width="50%" align="center">Upto</td>
        <td><vs-input type="date" class="w-full" size="small" v-model="date" /></td>
        </tr>
        <tr>
           <td id="overlap" class="div.example" align="center">State</td>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
           <td id="overlap" class="div.example" align="center"> Value by</td>
        <td id="overlap" class="div.example">
            <select class="w-full selectp">
                <option value="">With VAT</option>
                <option value=""></option>
            </select>
        </td>
        </tr>
        <tr>
           <td id="overlap" class="div.example" align="center">Tax Type</td>
        <td id="overlap" class="div.example">
            <select class="w-full selectp">
                <option value="">All</option>
                <option value=""></option>
            </select>
        </td>
        </tr>
      </table>
        </div>       
    </div><br><br><br>
    <div align="right" style="padding-top: 5px">
        <br>
      <div class="div.example">
        <br>
        <br>&nbsp;&nbsp;&nbsp;&nbsp;
            <vs-button  color="primary" type="filled">Edit</vs-button>&nbsp;
            <vs-button  color="primary" type="filled" style="!">Export</vs-button>&nbsp;
            <vs-button  color="primary" type="filled" style="!">Print</vs-button>&nbsp;        
      </div>
      </div>
</div>    
</template>






