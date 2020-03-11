<style>
.overlap
{
    max-width: 150px;
    max-height: 150px;
    overflow: hidden;
}




#page-wraps {
   
    width: 100%;
  
    position: relative;
    

}

#left1 {
    
    width: 25%;
    height: auto;
   
    float: left;
    padding-right: 1%;
    
    
}

#left2 {
    width: 25%;
    height: auto;
    float: left;
   
    padding-right: 1%;
  
}
#left3 {
    width: 25%;
    height: auto;
    float: left;
   
    padding-right: 1%;
  
}
#left4 {
    width: 25%;
    height: auto;
    float: left;
   
    padding-right: 1%;
  
}

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


.right {
  position: static;
  right: 0px;
  
  padding: 10px;
  
   width: 100%;
   min-width: 10px;  
   max-width: 300px;

}


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
#page-wraps {
   
    width: 100%;
  
    position: relative;
    

}

#left1 {
    
    width: 25%;
    height: auto;
   
    float: left;
    padding-right: 1%;
    
    
}

#left2 {
    width: 25%;
    height: auto;
    float: left;
   
    padding-right: 1%;
  
}
</style>
<style>
#tds_page-wrap {
   
    width: 100%;
  
    position: relative;
    

}

#tds_left {
    
    width: 50%;
    height: auto;
   
    float: left;
    padding-right: 1%;
    
    
}

#tds_right {
    width: 50%;
    height: auto;
    float: left;
    padding-bottom: 12%;
   
    padding-right: 1%;
  
}


#tds2_page-wrap {
   
    width: 100%;
    
    position: relative;
    height:auto;
    float: left;
    

}


#tds2_left {
    
    width: 30%;
    height: auto;
   
    float: left;
    padding-right: 1%;
    
    
}

#tds2_right {
    width: 70%;
    height: auto;
    float: left;
   
    padding-right: 1%;
  
}
td
{
    max-width: 150px;
    max-height: 150px;
    overflow: hidden;
}
#tds3_page-wrap {
   
     width: 100%;
    
    position: static;
    height:auto;
    float: right;
    
    
    

}
</style>

<template>

    <div class="vx-card p-6" style="" >
     <!--UPDATE START-->
      <table width="100%" border="0" class="tables">
     <tr>
      <td width="25%">
        
      </td>
       <td width="50%"><center><h1>Purchase State Wise Summary<br><h4><font color="blue">View</font></h4></h1></center></td>
       <td width="25%"  align="right">
           
                
              
        </td>
         
       


      </tr>
     
     
    
      </table>

         
    <!--UPDATE END-->
  
    <table border="0" width="100%" class="tables">
      
        <tr>
            <td width="30%" align="left">
                <table border="0" class="tables" align="left">
                <tr>
                <td class="overlap">
                From 
                </td>
                <td>
                 <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
                </td>
                
                </tr>

                 <tr>
                <td class="overlap">
               Upto 
                </td>
                <td>
                 <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
                </td>
                
                </tr>
               
               <tr>
                <td class="overlap">
               Agent
                </td>
                <td>
                 <vs-input class="w-full" size="small" v-model="input1" />
                </td>
                
                </tr>
               
                </table>


            </td>
            
           
            <td width="20%"></td>
        <td width="50%"  align="right">
           
                
              <div align="right">
       <div style=" position: static;
  right: 0px;
  
  padding: 10px;
  
   width: 100%;
   min-width: 10px;  
   max-width: 600px;" align="right">
         <vs-button  color="primary" type="filled">Display</vs-button>
        <br><br>
        <vs-button  color="primary" type="filled" style="!">Exit</vs-button>
        
        
         </div>
        </div>
            </td>
        </tr>
        
    </table>


   
<br>

	

 
    
    
    







<div style="overflow-x:auto;">  
<table id="customers" style="empty-cells:hide;">
  <tr>
    <th>Name of the State</th>
    <th>Pcs/Bags</th>
    <th>Quantity</th>
    <th>Value</th>
    
    
  </tr>
  <tr>
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
    
    
  </tr>
  <tr>
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
    
    
  </tr>
  <tr>
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
    
    
  </tr>
  <tr>
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
   
    
  </tr>
  
  
</table>



    </div>
       
      <div id="example">
        <!--IMPORT THE SCRIPT FOR ADDING ROWS AND USE THIS BUTTON-->
      <!--<button v-on:click="add_row">Add Row</button>-->
      
      <button class="btn"><i class="fa fa-plus"></i></button>

    </div> 

<table border="0" width="100%" class="tables">
<tr>
    <td width="40%"></td>
    <td width="60%">
        <table border="0" width="100%" class="tables">
            <tr>
                <td>Detail&nbsp;
                     <select class="w-full selectp">
            <option value="">Customer Wise Detail</option>
          </select>
       
                </td>
                <td>Total&nbsp;<vs-input class="w-full" size="small" v-model="input1" /></td>
            </tr>
        </table>
    </td>
</tr>
</table>





      
      
      
    </div>

    
</template>


