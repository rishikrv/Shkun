/* eslint-disable vue/valid-template-root */
<style>
.overlap {
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
.selectp {
  border-color: #7367f0;
  background-color: White;
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

#customers td,
#customers th {
  border: 1px solid #ddd;
}

#customers tr:nth-child(even) {
  background-color: #f2f2f2;
}

#customers tr:hover {
  background-color: #ddd;
}

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
    background-color: white;
    padding: 55px;

    border-color: #7367f0;
    border-top-style: solid;
    border-bottom-style: solid;
  }
}

@media screen and (max-width: 600px) {
  div.example {
    font-size: 10px;
    background-color: white;
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

.tables {
  table-layout: fixed;
  width: 100%;
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
  <div class="vx-card p-6" style>
    <!--UPDATE START-->
    <table width="100%" border="0" class="tables">
      <tr>
        <td width="100%">
          <center>
            <h1>
              Sale State Wise Sale
              <br />
            </h1>
          </center>
        </td>
      </tr>
    </table>

    <!--UPDATE END-->

  <br />

    <div id="page-wrap">
      <div id="rightt">
        <table border="0" width="100%" cellspacing="5" class="tables">
          <tr>
            <td class="overlap">From</td>
            <td>
              <vs-input type="date" class="w-full" size="small" v-model="mydate" />
            </td>
          </tr>
          <tr>
            <td class="overlap">Upto</td>
            <td>
             <vs-input type="date" class="w-full" size="small" v-model="mydate" />
            </td>
          </tr>
        </table>
      </div>
  

      <div id="mid">
        <table border="0" width="100%" cellspacing="5" class="tables">
           <tr>
            <td class="overlap">Agent</td>
            <td>
             <vs-input class="w-full" size="small" v-model="input1" />
            </td>
          </tr>
        </table>
      </div>
       
       <div id="example">
      <!--IMPORT THE SCRIPT FOR ADDING ROWS AND USE THIS BUTTON-->
      <!--<button v-on:click="add_row">Add Row</button>-->

      
              <vs-button color="primary" type="filled">Display</vs-button>&nbsp;
              <vs-button color="primary" type="filled">Print</vs-button>&nbsp;
              <vs-button color="primary" type="filled">Exit</vs-button>
    </div>
       
      <div style="clear:both;"></div>
    </div>
     <br/>
    <div style="overflow-x:auto;">
      <table id="customers">
        <tr>
          <th>Name of the State</th>
          <th>Pcs/Bage</th>
          <th>Ouantity</th>
          <th>Value</th>
        </tr>
        <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
        </tr>
        <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
        </tr>
        <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
        </tr>
        <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
        </tr>
       <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
        </tr>
                <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          
        </tr>
                <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
         
        </tr>
                <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          
        </tr>
                <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          
        </tr>
                <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
         
        </tr>
                <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
         
        </tr>
                <tr>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          <td>
            <vs-input class="w-full" size="small" v-model="input1" />
          </td>
          
        </tr>
      </table>
    </div>
     <br />

    <div id="page-wrap">
      <div>
        <table border="0" cellspacing="5" class="tables">
          <tr>
            <td class="overlap">Detail</td>
            <td>
              <select class="w-full selectp"><option value></option></select>
            </td>
            <td class="overlap">Total</td>
            <td>
              <vs-input class="w-full" size="small" v-model="input1" />
            </td>
          </tr>
        </table>
      </div>
    </div>
    <div align="right" style="padding-top: 80px">
      <br />
    </div>
  </div>
</template>