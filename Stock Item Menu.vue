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
      <h1>
        Stock Item Menu
        <br />
        <h4>View</h4>
      </h1>
    </center>

    <br />
    <table border="0" cellspacing="5" class="tables">
      <tr>
        <td>
          <input type="checkbox" />Carry Product Description
        </td>
      </tr>
      <tr>
        <td>A/c Code</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
        <td>
          <input type="checkbox" />Link With Ledger
        </td>
        <td>
          <input type="checkbox" />Stock Register
        </td>
      </tr>
      <tr>
        <td>Op.Stock in Qty</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td></td>
        <td>
          <input type="checkbox" />Active
        </td>
      </tr>
      <tr>
        <td>Box</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
        <td>Vehicle</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>Op.Stock in Rs</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
        <td>Scheme @</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>Group Name</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Expiry Dt</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
          <input type="checkbox" />On Qty
        </td>
      </tr>
      <tr>
        <td>Purchase Rate</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
        <td>Rate Calculater</td>
        <td>
          <select class="w-full">
            <option value="sdsdds"></option>
          </select>
        </td>
      </tr>
      <tr>
        <td>Less%</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Cls Stock in</td>
        <td>
          <select class="w-full">
            <option value="sdsdds"></option>
          </select>
        </td>
      </tr>
      <tr>
        <td>M.R.P</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Qty.in/UOM</td>
        <td>
          <select class="w-full">
            <option value="sdsdds"></option>
          </select>
        </td>
      </tr>
      <tr>
        <td>Less%</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td></td>
        <td>
          <select class="w-full">
            <option value="sdsdds"></option>
          </select>
        </td>
      </tr>
      <tr>
        <td>Sale Rate</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Stock Calculater</td>
        <td>
          <select class="w-full">
            <option value="sdsdds"></option>
          </select>
        </td>
      </tr>
      <tr>
        <td>Total GST @</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Type of Goods</td>
        <td>
          <select class="w-full">
            <option value="sdsdds"></option>
          </select>
        </td>
      </tr>
      <tr>
        <td>C.GST @</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Stk Valuation</td>
        <td>
          <select class="w-full">
            <option value="sdsdds"></option>
          </select>
        </td>
      </tr>
      <tr>
        <td>Cess Qty</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Qty Per Pc/Case</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>S.GST @</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Tariff Heading</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>Cess @</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Min.Stock Level</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>Purchase A/c</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td></td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>Sale A/c</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>GST Type</td>
        <td>
          <select class="w-full">
            <option value="sdsdds"></option>
          </select>
        </td>
      </tr>
      <tr>
        <td>Show in Excise</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td></td>
        <td>
          <vs-button class="mr-3 mb-2">Miscellaneous</vs-button>
        </td>
      </tr>
      <tr>
        <td>HSN Code</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td></td>
        <td>
          <input type="checkbox" />Add to Production Card
        </td>
      </tr>
      <tr>
        <td></td>
        <td>
          <vs-button class="mr-3 mb-2">F2-List</vs-button>
        </td>

        <td>Production Sr.No</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>Previous Purchase</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Unit No.</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
      </tr>
      <tr>
        <td>Previous Sale</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>

        <td>Percentage</td>
        <td>
          <vs-input class="w-full" size="small" v-model="input1" />
        </td>
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






