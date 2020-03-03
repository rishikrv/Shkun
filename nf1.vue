/* eslint-disable vue/valid-template-root */


<style type="text/css">


@media screen and (min-width: 601px) {
  div.example {
    font-size: 15px;
  }
}

@media screen and (max-width: 600px) {
  div.example {
    font-size: 10px;
  }
}

.btns {
   width: 100%;
   min-width: 10px;  
   max-width: 300px; 
   
}
</style>
<template>

    <div style="background:white">
    <center><h1><strong>Balance Sheet Annexture Form</strong> <br><h4><font color="7367f0">New</font></h4></h1></center>
    <br>
    
    <table border="0"  width="100%" >
      
        <tr align="center">
            <td width="100%">
                <table border="0">
                <tr>
                  <td width="0%">
                Name
                </td>
                <td >
                 <vs-input type="name"  size="small" v-model="name" />
                </td>
                <td>
                <vs-button class="mr-3 mb-2" style= "width:80px" size="small">Add</vs-button>
                </td>
                </tr>
                <tr>
                  <td>
                code
                </td>
                <td>
                 <vs-input type="name"  size="small" v-model="name" />
                </td>
                <td>
                <vs-button class="mr-3 mb-2" style= "width:80px" size="small">Edit</vs-button>
                </td>
                </tr>
                <tr>
                  <td>
               Detail in B/sheet
                </td>
                <td>
                 <vs-input type="name"  size="small" v-model="name" />
                </td>
                <td>
                <vs-button class="mr-3 mb-2" style= "width:80px"  size="small">Previous</vs-button>
                </td>
                </tr>
                <tr>
                  <td>
                Debit / Credit
                </td>
                <td>
                 <vs-input type="name"  size="small" v-model="name" />
                </td>
                <td>
                <vs-button class="mr-3 mb-2" style= "width:80px"  size="small">next</vs-button>
                </td>
                </tr>
                <tr>
                  <td>
                Description
                </td>
                <td>
                 <vs-input type="name"  size="small" v-model="name" />
                </td>
                <td>
                <vs-button class="mr-3 mb-2" style= "width:80px" size="small">Delete</vs-button>
                </td>
                </tr>
                <tr>
                  <td>
                Dr/Cr Effect
                </td>
                <td>
                 <vs-input type="name"  size="small" v-model="name" />
                </td>
                <td>
                <vs-button class="mr-3 mb-2" style= "width:80px" size="small">Save</vs-button>
                </td>
                </tr>
                <tr>
                  <td>
                Annual. Serial
                </td>
                <td>
                 <vs-input type="name"  size="small" v-model="name" />
                </td>
                <td>
                <vs-button class="mr-3 mb-2" style= "width:80px"  size="small">Exit</vs-button>
                </td>
                </tr>
                <tr>
                  <td>
                Group
                </td>
                <td>
                 <vs-input type="name"  size="small" v-model="name" />
                </td>
                <td>
                <vs-button class="mr-3 mb-2" style= "width:80px"  size="small">Print</vs-button>
                </td>
                </tr>
                </table>


            </td>
            
           
            
            <td width="80%"  align="right"><br> 
           
                
              
            </td>
        </tr>
        
    </table>

    <br>
    <br>    
    <h5> <b><center> NOTE: For New Group Please Click "Add" Button after Group where you adjust</center></b></h5>
    </div>
</template>
