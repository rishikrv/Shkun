/* eslint-disable vue/valid-template-root */
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
<form>
    <div class="vx-card p-6" style="" >
     <!--UPDATE START-->
      <table width="100%" border="0" class="tables">
     <tr>
      <td width="25%">
        
      </td>
       <td width="50%"><center><h1>Stock summary<br><h4><font color="blue">View</font></h4></h1></center></td>
       <td width="25%"  align="right">
        </td>
      </tr>
     
     
    
      </table>

         
    <!--UPDATE END-->

	<div id="page-wrap">

		<div id="left">
      <table border="0" width="100%" cellspacing="5" class="tables">
        <tr>
          <td class="overlap">From date</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
          <td class="overlap">Upto date</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
             
      </table>
    </div>
		
		<div id="rightt">
      <table border="0" width="100%" cellspacing="5" class="tables">
        <tr>
          <td class="overlap">Group</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
          <td class="overlap">Calculation</td>
          <td>
            <select class="w-full selectp">
            <option value=""></option>
          </select>
          </td>
        </tr>
        
        
      </table>
    </div>
			
        <div id="mid">
          <table border="0" width="100%" cellspacing="5"  class="tables">
        <tr>
          <td class="overlap">Filter</td>
          <td>
             <select class="w-full selectp">
            <option value=""></option>
          </select>
       
          </td>
        </tr>
        <tr>
          <td class="overlap">Order by</td>
          <td>
             <select class="w-full selectp">
            <option value=""></option>
          </select>
       
          </td>
        </tr>
        
        
      </table>
        </div>
       
		<div style="clear:both;"></div>
	</div>
<br>

	<table border="0" width="100%" class="tables">
        <tr>
            <td width="80%" align="left">
                <table border="0" class="tables" align="left">
                
                <tr>
                  <td>

                <div class="overlap">
                    <span><p>Method</p></span>
                </div>
                </td>
                <td>
                
                  <select class="w-full selectp">
                    <option></option>
                      </select>
                
                </td>
                 <td>

                <div class="overlap" align="right">
                    <span><p>Godown</p></span>
                </div>
                </td>
                <td>
                 <vs-input class="w-full"  size="small" v-model="input1"/>
                  </td>
                
                
                </tr>
                </table>


            </td>
            
           
            <td width="10%"></td>
      <td width="50%"  align="right">
           
                
              <div align="right">
       
        </div>
            </td>
        </tr>
        
    </table>

   

<br>
<div style="overflow-x:auto;">  
<table id="customers">
  <tr>
    <th>Account Name</th>
    <th>Op.</th>
    <th>Opening</th>
    <th>Rec.</th>
    <th>Rec.Qty</th>
    <th>Issue</th>
    <th>Issue Qty</th>
    <th>cls.</th>
        <th>Closing</th>
            <th>Values</th>
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
       
        <td>Search
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
          <td></td>

          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
         <td><vs-input class="w-full" size="small" v-model="input1" /></td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
      </tr>
      <td>A/c code
         <td><vs-input class="w-full" size="small" v-model="input1" /></td>


      
    </table>
    </div>
    
    </div>




    
      <!--
      <table width="100%">
      <tr>
        <td width="80%"></td>
        <td width="10%">
      
        <vs-button  color="primary" type="filled">Edit</vs-button>
        
      </td>
      <td  width="10%">
        <vs-button  color="primary" type="filled" style="!">Export</vs-button>
      </td>
      </tr>
      </table>
      -->
      <div >
        <br>

      <div class="right" align="center">
        <br>
        <table border="0" width="100%" align="center">
        <tr>
        <td align=""><vs-button  color="primary" type="filled">Edit</vs-button></td>
      
        <td><vs-button  color="primary" type="filled" style="!">Export</vs-button></td>
      
        <td><vs-button  color="primary" type="filled">Refresh</vs-button></td>
      
        <td><vs-button  color="primary" type="filled">Print</vs-button></td>
        
        <td><vs-button  color="primary" type="filled">Exit</vs-button></td>
        </tr>
        </table>
      
        

      </div>
      </div>
      
      
      
    </div>

    </form>
</template>













