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
    padding-right: 70%;
    
    
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
 
  width: 50%;
  
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
td.hiden{
  visibility: hidden;
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
       <td width="50%"><center><h1>Passbook Feeding<br><h4><font color="blue">View</font></h4></h1></center></td>
        <td width="25%"  align="right"><br>     
        </td>
      </tr>
      </table>

         
    <!--UPDATE END-->
  
    <table border="0" width="100%" class="tables">
      
        <tr>
            <td width="60%" align="left"  style="padding-right:">
              <table border="0" class="tables" align="left">
                <tr>
                <td class="overlap" align="center">
                  <div id="example">
                      <button class="btn"><i class="fa fa-trash"></i></button>
                  </div> 
                </td>
                </tr>
                <tr>
                  <td  align="center" class="overlap">
                    <div id="example">
                        <button class="btn" ><i class="fa fa-thumbs-up"></i></button>
                    </div>
                  </td>
                        
                  <td class="overlap" width="20%" align="right">
                      Date
                  </td>
                  <td>
                    <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
                  </td>
      
                </tr>
                <tr>
                  <td class="overlap">
                      <div id="example" align="center">
                          <button class="btn"><i class="fa fa-close"></i></button>
                      </div>
                  </td>
                  <td class="overlap" width="20%" align="right">
                      V.No
                  </td>
                  <td>
                    <vs-input class="w-full"  size="small" v-model="input1"/>
                  </td>
                </tr>
                <br>
                <tr>
                    <td class="overlap,tables" align="right">
                      <td width="80%"><center><h4>Interest Calculation</h4></center>
                    </td>
                </tr>
                <br>
                <tr>
                  <td class="overlap" width="100%" align="center" id="">
                   
                      <button class="btn" id="tables">Interest Report</button>
                  
                  </td>
                  <td class="overlap" align="right" id="tables" width="80%">From</td>
                  <td align="center"><vs-input class="w-full" size="small" v-model="input1" /></td>
                </tr>
                <tr>
                  <td class="overlap" id="tables" >
                      <div id="example">
                         
                      </div>
                  </td>
                  <td class="overlap" align="right"  width="10%">Upto</td>
                  <td ><vs-input class="w-full" size="small" v-model="input1" /></td>
                </tr>
                <tr>
                  <td class="overlap">
                      <div id="example">
                         
                      </div>
                  </td>
                  <td class="overlap" align="right"  width="10%">Intt.@</td>
                  <td align="left"><vs-input type="label" class="w-full" size="small" v-model="label" /></td>
                </tr>
            </table>
            </td>
            
         
        <td width="40%"  align="right">      
          <div align="right" style="overflow-x:auto;overflow-y:auto">
            <div class="right" align="right">
              <table border="0" width="100%" cellspacing="5"  class="tables" id="customers">
                <tr>
                    <th>Date</th>
                    <th>Balance</th> 
                </tr>
                <tr>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                </tr>
                <tr>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                </tr>
                <tr>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                </tr>
                 <tr>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                </tr>
                <tr>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                </tr>
                <tr>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
                </tr>
              </table> 
              <div id="example">
                <button class="btn"><i class="fa fa-plus"></i></button>
              </div>
            
            </div>
          </div>
        </td>
        </tr> 
    </table>    
    </div>
</template>






