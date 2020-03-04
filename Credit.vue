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
<style>
        .container {
            max-width: 930px;
            margin: 0px auto;
            margin-top: 50px;
        }

        .comment {
            float: left;
            width: 100%;
            height: auto;
        }

        .commenter {
            float: left;
        }

        .commenter img {
            width: 35px;
            height: 35px;
        }

        .comment-text-area {
            float: left;
            width: 100%;
            height: auto;
        }

        .textinput {
            float: left;
            width: 100%;
            min-height: 300px;
            outline: none;
            resize: none;
            border: 1px solid grey;
        }
    </style>

<template >

    <div class="vx-card p-6" style=""  >
     <!--UPDATE START-->
    <table width="100%" border="0" class="tables">
         <tr>
           
            <td width="10%">   
            </td>
            <td width="50%"><center><h1>Credit Note<br><h4><font color="blue">View</font></h4></h1></center></td>
       <td width="25%"  align="right"><h6>Edge on ledger</h6>
       <tr>
          
          <td>
             <select class="w-full selectp">
            <option value="">Yes</option>
            <option value="">No</option>
          </select>
       
          </td>
          </tr>
          </td>
          </tr>
     
    </table>

         
    <!--UPDATE END-->
    <br>
     <table border="0" width="100%" class="tables">
        <tr>
            <td width="80%" align="left">
                <table border="0" class="tables" align="left">
                <tr>
                <td class="overlap">
                  Date
                </td>
                <td class="overlap"> 
                 <vs-input type="date" class="w-full"  size="small" v-model="mydate"/>
                </td>
                
                </tr>
                <tr>
                  <td>

                <div class="overlap">
                    <span><p>V.No</p></span>
                </div>
                </td>
                <td>
                
                     <vs-input class="w-full" size="small" v-model="input1" />
                
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

	<table border="0" width="100%" class="tables">
        <tr>
            <td width="80%" align="left">
                <table border="0" class="tables" align="left">
                
                <tr>
                  <td>

                <div class="overlap">
                    <span><p>Credit</p></span>
                </div>
                </td>
                <td>
                
                     <vs-input class="w-full" size="small" v-model="input1" />
                
                </td>
                
                
                </tr>
                <tr>
                  <td>

                <div class="overlap">
                    <span><p>Debit</p></span>
                </div>
                </td>
                <td>
                
                     <vs-input class="w-full" size="small" v-model="input1" />
                
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
<table border="0" width="100%" class="tables">
        <tr>
            <td>
              <table border="0" class="tables" align="top" style="padding-bottom:10px">
                  <tr>
                  <td width="20%" class="overlap" style="padding-bottom:200px">
                    Details
                  </td>
                  <td width="80%">
                    <div class="container">
                      <div class="comment">
                        <textarea class="textinput"></textarea>
                      </div>
                    </div>
                  </td>
                  </tr>
                </table>
                 
                  <table border="0" class="tables" style="padding-bottom:1000px">
                  <tr>
                  <td class="overlap" align="left" id="tables">Qty</td>
                  <td ><vs-input class="w-full" size="small" v-model="input1" /></td>
                  <td class="overlap" align="right" id="tables">Amount</td>
                  <td ><vs-input class="w-full" size="small" v-model="input1" /></td>
                  </tr> 
                  <tr>
                  <td class="overlap" align="left" id="tables" width="10%">Rate</td>
                  <td ><vs-input class="w-full" size="small" v-model="input1" /></td>
                  </tr>  
              </table>
            </td>
            
         
        <td width="40%"  style="padding-bottom:900px">      
          <div  >
            <div  >
              <table border="0" width="100%" cellspacing="5" class="tables">
                <tr >
                <td align="center"> 
                <button class="btn"><i class="fa fa-plus"></i></button>
                </td>
                <td align="center"> 
                <button class="btn"><i class="fa fa-edit"></i></button>
                </td>
                </tr>
                <tr>
                <td align="center"> 
                <button class="btn"><i class="fa fa-floppy-o"></i></button>
                </td>
                <td align="center"> 
                <button class="btn"><i class="fa fa-trash"></i></button>
                </td>
                </tr>
                </table>
               <table border="0" width="100%" cellspacing="5" class="tables">
                <tr  >
                  <td  align="center">
                    <button class="btn"><i class="fa fa-search" ></i></button>
                  </td>
                </tr>
                </table>
                <table border="0" width="100%" cellspacing="5" class="tables">
                <tr>
                  <td align="center">
                    <button class="btn"><i class="fa fa-step-backward"></i></button>
                  </td>
                  <td align="center" >
                    <button class="btn"><i class="fa fa-angle-left"></i></button>
                  </td>
                  <td align="center" >
                    <button class="btn"><i class="fa fa-angle-left"></i></button>
                  </td>
                  <td align="center" >
                    <button class="btn"><i class="fa fa-step-forward"></i></button>
                  </td>
                </tr>
                </table>
               <table border="0" width="100%" cellspacing="5" class="tables">
                <tr>
                  <td align="center" width="90%" >
                    <button class="btn"><i class="fa fa-question"></i></button>
                  </td>
                  
                </tr>

              </table> 
             
            
            </div>
          </div>
        </td>
        </tr> 
    </table>   
    </div>

    
</template>






