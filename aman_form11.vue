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
</style>

<template>

    <div class="vx-card p-6" style="" >
     <!--UPDATE START-->
      <table width="100%" border="0" class="tables">
     <tr>
      <td width="25%">
        
      </td>
       <td width="50%"><center><h1>Sale Summary<br></h1></center></td>
       <td width="25%"  align="right">
           
                
              
        </td>
         
       


      </tr>
     
     
    
      </table>
        <br>

      <div id="tds2_page-wrap">
      <div id="tds_left" style="padding-right:3%;">
      <table width="100%" border="0" class="tables" cellspacing="5">
        <tr>
          <td>From</td>
          <td><vs-input type="date" class="w-full"  size="small" v-model="mydate"/></td>
        </tr>
        <tr>
          <td>Upto</td>
          <td><vs-input type="date" class="w-full"  size="small" v-model="mydate"/></td>
        </tr>
        <tr>
          <td>City Name</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
          <td>State</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
          <td>Agent <input type="checkbox">B2B</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
          <td>Value By</td>
          <td>
              <select class="w-full selectp">
            <option value="">With VAT</option>
          </select>
            </td>
        </tr>
        <tr>
          <td>Full Address</td>
          <td>
              <select class="w-full selectp">
            <option value="">Yes</option>
          </select>
            </td>
        </tr>
        <tr>
          <td>Tax Type</td>
          <td>
              <select class="w-full selectp">
            <option value="">All</option>
          </select>
            </td>
        </tr>
        <tr>
          <td>Product Comp</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
      </table>
      </div>

      <div id="tds_right" style="padding-bottom:12px; padding-left:3%;">
        <table width="100%" border="0" class="tables" cellspacing="5">
        <tr>
          <td>
            <input type="radio"> &nbsp; Total Summary
          </td>
          <td></td>
        </tr>
        <tr>
          <td>
            <input type="radio"> &nbsp; Month Wise
          </td>
          <td></td>
        </tr>
        <tr>
          <td>
            <input type="radio"> &nbsp; Date Wise
          </td>
          <td></td>
        </tr>
        <tr>
          <td>
            <input type="radio"> &nbsp; Certificate
          </td>
          <td></td>
        </tr>
        <tr>
          <td>
            Minimum Qty
          </td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
          <td>
            Maximum Qty
          </td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
          <td>
            Minimum Value
          </td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
          <td>
            Maximum Value
          </td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        </table>
        <table width="100%" border="0" class="tables" cellspacing="5">
        <tr>
        <td align="center">
         <vs-button  color="primary" type="filled" style="!">Select Ledger Accounts</vs-button>
         </td>
         </tr>
         <tr>
           <td align="center">
         <vs-button  color="primary" type="filled" style="!">Select Stock Items</vs-button>
            </td>
        </tr>
        <tr>
          <td align="center">
        <input type="checkbox"> &nbsp; <font color="red">Less Dr/Cr Note</font>
          </td>
        </tr>
        </table>
      </div>
      </div>
        
        
        <div align="right" style="padding-top: 1px">
      <br>

      <div style="position: static;
  right: 0px;
  padding: 1px;
   width: 100%;
   min-width: 10px;  
   max-width: 300px;" align="center">
        <br>
        
        <vs-button  color="primary" type="filled" style="!">Print</vs-button>
         &nbsp;
        <vs-button  color="primary" type="filled" style="!">Export</vs-button>
        

      </div>
      </div>

    <br>

      
      
      
      
      
    </div>

    
</template>

