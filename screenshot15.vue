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
      <td width="25%">
        
      </td>
       <td width="50%"><center><h1>Voucher Printing Options<br><h4><font color="blue"></font></h4></h1></center></td>
       <td width="25%"  align="right">Today 25-10-2020 <br> Thursday
           
                
              
        </td>
         
       


      </tr>
     
     <br>
    
      </table>
      <table width="100%" border="0" class="tables">
     <tr>
      <td width="35%">
          <br>
               <br>
           <tr>
               
               
                <td>
                Period  From
                </td>
                <td >
                 <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
                </td>
                </tr>
                
                <tr>
                <td>
               Upto
                </td>
                <td >
                 <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
                </td>
                </tr>
                <br>
                <br>
                <br>
                <br>
                <br>
               
        
      </td>
       <td width="30%">
           <br>
           <br>
           <br>
           <br>
           <br>
           <br>
      

           <h4 align="center"><font color="blue">Vouchers</font></h4></td>
       <td width="35%"  align="left">
            <tr>
                <td>

                    <vs-checkbox v-model="checkBox">Cash</vs-checkbox>


  </td>
               
                </tr>
                 <tr>
                <td>

                    <vs-checkbox v-model="checkBox">Journal</vs-checkbox>


  </td>
               
                </tr>
                 <tr>
                <td>

                    <vs-checkbox v-model="checkBox">Bank</vs-checkbox>


  </td>
               
                </tr>
                 <tr>
                <td>

                    <vs-checkbox v-model="checkBox">Sale</vs-checkbox>


  </td>
               
                </tr>
                 <tr>
                <td>

                    <vs-checkbox v-model="checkBox">Purchase</vs-checkbox>


  </td>
               
                </tr>
                 <tr>
                <td>

                    <vs-checkbox v-model="checkBox">TDS</vs-checkbox>


  </td>
               
                </tr>
           
                
              
        </td>
         
       


      </tr>
     
     
    
      </table>

      

     <table border="0"  width="100%" >
      
        <tr align="right">
            <td width="100%">
                <table border="0">
                <tr>

               
                <td>
                <vs-button class="mr-3 mb-2" style= "width:80px" size="small">Cancel</vs-button>
                </td>
                <td>
                <vs-button class="mr-3 mb-2" style= "width:80px" size="small">Ok</vs-button>
                </td>
               

                </tr>
                </table>
                </td>
                </tr>
                </table>
    
    
    </div>

    
    </template>