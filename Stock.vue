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

     <div class="vx-card p-6" style="" >
     <!--UPDATE START-->
      <table width="100%" border="0" class="tables">
     <tr>
      <td width="25%">
        
      </td>
       <td width="50%"><center><h1>Stock Summary<br><h4><font color="blue">View</font></h4></h1></center></td>
       <td width="25%"  align="right">  
          <div align="right">
      <div class="right" align="center">
        <button class="btn"><i class="fa fa-flag"></i></button>

      </div>
      </div>
        </td>
         
       


      </tr>
     
     
    
      </table>
    <!--UPDATE END-->
    <br>
    <div>
        <tr>
            <td  align="left">
                <table border="0" class="tables" align="100%">
                <tr>
                <td width="15%">
                  From Date
                </td>
                <td class="overlap" > 
                 <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
                </td>
                <td  width="3%" >
                <vs-input type="checkbox" class="w-full"  size="small" v-model="checkbox"/>
                </td>
                <td  class="overlap">
                    HSN
                </td>
                <td class="overlap" align="right" >
                    Group

                </td>
                <td class="overlap" > 
                 <vs-input class="w-full"  size="small" v-model="input1"/>
                </td>
                <td  id="overlap" align="right">
                    Filter
                </td>
                <td>
                        <select class="w-full selectp">
                        <option value=""></option>
                        <option value=""></option>
                        </select>
                </td> 
                </tr>
                <tr>
                <td>
                    Upto Date
                </td>
                 <td class="overlap"> 
                 <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
                </td>
                <td>
                </td>
                <td>
                </td>
                <td id="overlap" align="right" width="20%">
                    Calculation
                </td>
                <td>
                        <select class="w-full selectp">
                        <option value=""></option>
                        <option value=""></option>
                        </select>
                </td> 
                <td id="overlap" align="right">
                    Order By
                </td>
                <td>
                        <select class="w-full selectp">
                        <option value=""></option>
                        <option value=""></option>
                        </select>
                </td> 
                </tr>
                </table>
            </td>
        </tr>
    </div>

<table border="0" width="100%" class="tables">
        <tr>
            <td width="15%" class="overlap">
                Method
            </td>
            <td  width="14%">
              <select class="w-full selectp">
                <option value="">Default</option>
                <option value=""></option>
              </select>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
            </td>
        </tr>
</table>
<div style="overflow-x:auto;" >  
<table id="customers">
  <tr>
    <th>Account Name</th>
    <th>Opening</th>
    <th>Receipt</th>
    <th>Issue</th>
    <th>Closing</th>
    <th>Rate</th>
    <th>Value</th>
    <th>Discount</th>
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
  </tr>
<div id="example">
  <button class="btn"><i class="fa fa-plus"></i></button>
  
</div> 
</table>
</div>
<br>
<table border="0"  width="100%" cellspacing="5" class="tables" >
  <tr>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        <td><vs-input class="w-full" size="small" v-model="input1" /></td>
  </tr>
</table>
<br>
<table border="0" width="100%" >
  <tr>
    <td align="right"> 
      Search
    </td>
    <td align>
      <vs-input class="w-full" size="small" v-model="input1" />
    </td>
    <td width="5%" >
      <vs-input type="checkbox" class="w-full"  size="small" v-model="checkbox"/>
    </td>
    <td class="overlap"><font color="red">
      Filter Selected Item
    </font></td>
  </tr>
  <tr>
    <td width="20%" align="right">
      A/c Code
    </td>
    <td align>
      <vs-input class="w-full" size="small" v-model="input1" />
    </td>
    <td width="5%" >
      <vs-input type="checkbox" class="w-full"  size="small" v-model="checkbox"/>
    </td>
    <td class="overlap" ><font color="red">
      Negative Stock Status
    </font></td>
      <td  align="center" class="mid" >
        <div id="example" width="70%" >
          <button class="btn"><i class="fa fa-pencil"></i></button>
      </div>
    </td>
    <td  align="center">
      <div id="example">
        <button class="btn"><i class="fa fa-print"></i></button>
      </div>
    </td>
    <td  align="center" width="10%">
      <div id="example">
        <button class="btn"><i class="fa fa-save"></i></button>
      </div>
    </td>
  </tr>
  <tr>
    <td align="right">
    Filter
    </td>
    <td align="center">
      <vs-input class="w-full" size="small" v-model="input1" />
    </td>
    <td width="1%" >
      <vs-input type="checkbox" class="w-full"  size="small" v-model="checkbox"/>
    </td>
    <td class="overlap">
      Filter Selected Item
    </td>
    <td>
    </td>
    <td>
    </td>

  </tr>   
</table>
</div>    
</template>






