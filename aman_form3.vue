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
       <td width="50%"><center><h1>TDS Voucher<br><h4><font color="blue">View</font></h4></h1></center></td>
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
                Vch.Date
                </td>
                <td>
                 <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
                </td>
                
                </tr>
                <tr>
                  <td>

        
                 
                <div class="vx-col sm:w-1/3 w-full overlap">
                    <span><p>Vch.No</p></span>
                </div>
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
       <div class="right" align="right">
        <button class="btn"><i class="fa fa-cog"></i></button>
        &nbsp;
        <button class="btn"><i class="fa fa-bars"></i></button>
        
         </div>
        </div>
            </td>
        </tr>
        
    </table>


   
<br>

	<div id="tds_page-wrap">

		<div id="tds_left">
      <table border="0" width="100%" cellspacing="5" class="tables">
        <tr>
          <td class="overlap">Credit A/c</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
          <td class="overlap">City</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
          <td class="overlap">TDS on</td>
          <td>
                  <select class="w-full selectp">
            <option value=""></option>
          </select>
       
            </td>
        </tr>
        <tr>
          <td class="overlap">TDS Ret A/c</td>
          <td>
       <vs-input class="w-full" size="small" v-model="input1" />
            </td>

        </tr>
        <tr>
          <td class="overlap">P.A.N</td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
            </td>

        </tr>
      </table>
    </div>
		
		<div id="tds_right">
      <table border="0" width="100%" cellspacing="5" class="tables">
        <tr>
          <td class="overlap">Debit A/c</td>
          <td><vs-input class="w-full" size="small" v-model="input1" /></td>
        </tr>
        <tr>
          <td class="overlap">City</td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
        </tr>
        <tr>
          <td class="overlap">Tds A/c</td>
          <td>

                 <select class="w-full selectp">
            <option value=""></option>
          </select>
       
          </td>
        </tr>
        
      </table>
    </div>
		
	</div>

 
    
    
    





<br>

<div  id="tds2_page-wrap">
<div id="tds2_left">

<table width="100%" border="0" class="tables">
  <tr>
    <td>Amount</td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
  </tr>
  <tr>
    <td>Other Exp.</td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
  </tr>
  <tr>
    <td>Vehicle No.</td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
  </tr>
  <tr>
    <td>Gr No.</td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
  </tr>
  <tr>
    <td>GR Date</td>
    <td>
      <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
    </td>
  </tr>
  <tr>
    <td>Invoice No.</td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
  </tr>
  <tr>
    <td>Invoice Dt.</td>
    <td><vs-input type="date" class="w-full"  size="small" v-model="mydate"/></td>
  </tr>
  <tr>
    <td>Weight</td>
    <td><vs-input class="w-full" size="small" v-model="input1" /></td>
  </tr>

</table>
  </div>
  <div id="tds2_right">
    <table border="1" width="100%" class="tables" style="border-color:#7367f0;" >
      <tr>
        <td>
          <table width="100%" border="0" class="tables" style="padding:2%;">
            <tr>
              <td></td>
              <td>Rate</td>
              <td>Value</td>

            </tr>
            <tr>
              <td>T.D.S</td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>

            </tr>
            <tr>
              <td>Sur.@</td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>

            </tr>
            <tr>
              <td>Cess</td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>

            </tr>
            <tr>
              <td>HE.Cess</td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>

            </tr>
            <tr>
              <td></td>
              <td>Total</td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>

            </tr>
          </table>

          <table width="100%" border="0" class="tables" style="padding:2%;">
            <tr>
              <td class="overlap">Deposit Dt.</td>
              <td class="overlap">Challan No.</td>
              <td class="overlap">Cheque No</td>
            </tr>
            <tr>
              <td><vs-input type="date" class="w-full"  size="small" v-model="mydate"/></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
            </tr>

            </table>
            <table width="100%" border="0" class="tables" style="padding:2%;">
              <tr>
                <td>Bank</td>
                <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              </tr>
              <tr>
                <td>Led. Post</td>
                <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              </tr>
            </table>

        </td>
        <td>
           <table width="100%" border="0" class="tables" style="padding:2%;">
            <tr>
              <td></td>
              <td>Rate</td>
              <td>Value</td>

            </tr>
            <tr>
              <td>C.Tax</td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>

            </tr>
            <tr>
              <td>S.Tax</td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>

            </tr>
            <tr>
              <td>I.Tax</td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>

            </tr>
            <tr>
              <td>Cess</td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>

            </tr>
            <tr>
              <td></td>
              <td>Total</td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>

            </tr>
          </table>
          <table width="100%" border="0" class="tables" style="padding:2%;">
            <tr>
              <td class="overlap">Deposit Dt.</td>
              <td class="overlap">Challan No.</td>
              <td class="overlap">Cheque No</td>
            </tr>
            <tr>
              <td><vs-input type="date" class="w-full"  size="small" v-model="mydate"/></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              <td><vs-input class="w-full" size="small" v-model="input1" /></td>
            </tr>

            </table>
            <table width="100%" border="0" class="tables" style="padding:2%;">
              <tr>
                <td>St. Payable</td>
                <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              </tr>
              <tr>
                <td>Led. Post</td>
                <td><vs-input class="w-full" size="small" v-model="input1" /></td>
              </tr>
            </table>
        </td>

      </tr>
    </table>

    







    
  </div>
  
</div>

 <table>
      <tr>
        <td>
          Pur. Party
          <select class="w-full selectp">
            <option value=""></option>
          </select>
       

        </td>
        <td>
          Ledger Posting
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
    </table>




      
      <div align="right" style="padding-top: 10px">
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






