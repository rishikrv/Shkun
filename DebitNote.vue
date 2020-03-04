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
    
    width: 50%;
    height: auto;
   
    float: left;
    padding-right: 8%;
    
    
}

#mid {
    width: 50%;
    height: auto;
    float: left;
   
    padding-left: 8%;
  
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

<template >

    <div class="vx-card p-6" style=""  >
     <!--UPDATE START-->
    <table width="100%" border="0" class="tables">
         <tr>
           
            <td width="10%">   
            </td>
            <td width="80%"><center><h1>Debit Note<br><h4><font color="blue">View</font></h4></h1></center></td>
            <td>   
            </td>
        
         </tr>
     
    </table>

         
    <!--UPDATE END-->
  
    <table border="0" width="100%" class="tables">
      
        <tr>
            <td width="25%" align="left">
                <table border="0" class="tables" align="left">
                    <tr>
                        <td class="overlap">
                            Date 
                        </td>
                        <td>
                        <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
                        </td>
                
                    </tr>
                    <tr>
                        <td>
                            <div class="vx-col sm:w-1/3 w-full overlap">
                            <span><p>V.No</p></span>
                            </div>
                        </td>
                        <td>
                            <vs-input class="w-full" size="small" v-model="input1" />
                        </td>
                    </tr>
                </table>


            </td>
            
           
            <td width="65%"></td>
            <td width="10%"  align="right">
           
                
                <div align="right">
                    <div class="right" align="right">
                        <tr>
                        <td width="10%"  align="right">Effect on Ledger</td></tr>
                        <tr>
                            <td> <select  class="w-full selectp" >
                        <option value=""></option></select>
                        </td>
                        </tr>
        
                    </div>
                </div>
            </td>
        </tr>
        
    </table>


   
<br>
<table width="65%" border="0">
    <tr>
    
          <td width="19%">
             Debit
          </td>
           <td  width="46%"><vs-input class="w-full" size="small" v-model="input1" /></td>
           
           <br>
           
         
    
    </tr>
    <tr>
        
          <td >
              Credit
          </td>
           <td ><vs-input class="w-full" size="small" v-model="input1" /></td>
           
           

    
        </tr>
    
    

</table>	
<table border="0">

<tr>
        
          <td width="17%"  >
               Details
                 
              
          </td>
           <td  width="37%"><textarea rows="10" cols="80">
               </textarea>
           </td>
           
           <td  width="23%">
           </td>
           <td  width="23%">
           </td>
           

    
        </tr>	
		
</table>		
        



       
      
<div style="overflow-x:auto;"  width="100%">  
      <table>
  
        <tr>
         <td class="hiden" width="9%"></td>
          <td class="hiden" width="9%"></td>
          <td width="8.3%">Qty.t</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
           
          
          <td class="hiden" width="9%"></td>
           <td width="8.3%">Value</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
          
          <td class="hiden" width="8.3%"></td>
         
          
          
         
        </tr> 
        <tr>
         <td class="hiden" width="9%"></td>
          <td class="hiden" width="9%"></td>
          <td width="8.3%">Qty.t</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td></tr>
 
  
      </table>



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
      -->
      <div align="right" style="padding-top: 20px">
        <br>

      <div class="right" align="right">
        <br>
        <vs-button  color="primary" type="filled">Print</vs-button>
        &nbsp;
        <vs-button  color="primary" type="filled" style="!">Submit</vs-button>
        

      </div>
      </div>
      
      
      
    </div>

    
</template>






