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
    <center>
      <h1>LOANS & ADVANCES</h1>
    </center>

    <br />
    <table width="100%" border="0" class="tables">
       <tr>
        <td>A/c Code</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
        <td></td>
        <td>
          Today 25-10-2020
        </td>
      </tr>
       <tr>
        <td>A/c Name</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
        <td></td>
        <td>
          Thursday
        </td>
      </tr>
      <tr>
        <td>Address</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
        <td>RC No.</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td></td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Range</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>City</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
        <td>Division</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>PinCode</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
       
        <td>Collectorate</td>
        <td>
         <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
         <td>Distt.</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
        <tr>
        <td>GST No.</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>SAC Code</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>State</td>
        <td>
          <select class="w-full"><option value="sdsdds"></option></select>
        </td>
        <td></td>
        <td>
          <vs-button class="mr-3 mb-2">Misc. Information / Attach Image</vs-button>
        </td>
      </tr>
      <tr>
        <td>
          Distance
        </td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr> 
      <tr>
        <td>Opening Balance Dr</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Contact Person</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>Opening Balance Cr</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Intt/Depc.Rate</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>Contact No.</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>TDS Rate</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
    </tr>
	<tr>
        <td>M.Email ID / Area</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>GST / Share%</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
    </tr>
	<tr>
        <td>Agent / Group</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Quantitiy</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
    </tr>
	<tr>
        <td>PAN</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Bank A/c No.</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
    </tr>
	<tr>
        <td>TDS A/c No.</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Composition Y/N</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
    </tr>
	<tr>
        <td>Works</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td></td>
        <td>
         
        </td>
    </tr>
	<tr>
        <td>Name & Address</td>
        <td>
           <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td></td>
    </tr>
    <tr>
        <td>Name & Address</td>
        <td>
           <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td></td>
    </tr>
    </table>
     <div align="right" style="padding-top: 170px">
        <div class="right" align="right">
        <vs-button color="primary" type="filled">Print</vs-button>&nbsp;
        <vs-button color="primary" type="filled" style="!">Submit</vs-button>
      </div>
    </div>
  </div>
</template>






