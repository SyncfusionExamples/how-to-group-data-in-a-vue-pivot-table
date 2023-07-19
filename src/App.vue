<script>
  import { PivotViewComponent, GroupingBar, Grouping } from "@syncfusion/ej2-vue-pivotview";
  
export default{
  components: {
    "ejs-pivotview": PivotViewComponent
  },
  data()
  {
    return{
      dataSourceSettings:{
        dataSource:[
        {
            "Date": new Date(2015,0,1),
            "Product_Categories": "Accessories",
            "Product_ID": 1001,
            "Sold": 6,
            "Products": "Bottles and Cages",
            "Amount": 12
        },
        {
            "Date": new Date(2015,0,2),
            "Product_Categories": "Accessories",
            "Product_ID": 1002,
            "Sold": 9,
            "Products": "Cleaners",
            "Amount": 27
        },
        {
            "Date": new Date(2015,0,3),
            "Product_Categories": "Accessories",
            "Product_ID": 1003,
            "Sold": 15,
            "Products": "Fenders",
            "Amount": 120
        },
        {
            "Date": new Date(2015,0,4),
            "Product_Categories": "Bikes",
            "Product_ID": 1004,
            "Sold": 3,
            "Products": "Mountain Bikes",
            "Amount": 180
        },
        {
            "Date": new Date(2015,0,5),
            "Product_Categories": "Bikes",
            "Product_ID": 1005,
            "Sold": 3,
            "Products": "Road Bikes",
            "Amount": 225
        },
        {
            "Date": new Date(2015,1,11),
            "Product_Categories": "Clothings",
            "Product_ID": 1007,
            "Sold": 6,
            "Products": "Gloves",
            "Amount": 18
        },
        {
            "Date": new Date(2015,1,12),
            "Product_Categories": "Clothings",
            "Product_ID": 1008,
            "Sold": 3,
            "Products": "Jerseys",
            "Amount": 15
        },
        {
            "Date": new Date(2015,1,13),
            "Product_Categories": "Clothings",
            "Product_ID": 1009,
            "Sold": 9,
            "Products": "Shorts",
            "Amount": 36
        },
        {
            "Date": new Date(2015,1,14),
            "Product_Categories": "Accessories",
            "Product_ID": 1003,
            "Sold": 9,
            "Products": "Fenders",
            "Amount": 72
        },
        {
            "Date": new Date(2015,1,15),
            "Product_Categories": "Accessories",
            "Product_ID": 1002,
            "Sold": 12,
            "Products": "Cleaners",
            "Amount": 36
        },
        {
            "Date": new Date(2015,2,1),
            "Product_Categories": "Accessories",
            "Product_ID": 1002,
            "Sold": 3,
            "Products": "Cleaners",
            "Amount": 9
        },
        {
            "Date": new Date(2015,2,2),
            "Product_Categories": "Bikes",
            "Product_ID": 1001,
            "Sold": 9,
            "Products": "Mountain Bikes",
            "Amount": 540
        },
        {
            "Date": new Date(2015,2,2),
            "Product_Categories": "Bikes",
            "Product_ID": 1004,
            "Sold": 9,
            "Products": "Mountain Bikes",
            "Amount": 540
        },
        {
            "Date": new Date(2015,2,3),
            "Product_Categories": "Bikes",
            "Product_ID": 1005,
            "Sold": 6,
            "Products": "Road Bikes",
            "Amount": 450
        },
        {
            "Date": new Date(2015,2,4),
            "Product_Categories": "Bikes",
            "Product_ID": 1006,
            "Sold": 12,
            "Products": "Touring Bikes",
            "Amount": 780
        },
        {
            "Date": new Date(2015,2,5),
            "Product_Categories": "Clothings",
            "Product_ID": 1008,
            "Sold": 24,
            "Products": "Jerseys",
            "Amount": 120
        },
        {
            "Date": new Date(2015,2,11),
            "Product_Categories": "Clothings",
            "Product_ID": 1009,
            "Sold": 3,
            "Products": "Shorts",
            "Amount": 12
        },
        {
            "Date": new Date(2015,2,10),
            "Product_Categories": "Clothings",
            "Product_ID": 1010,
            "Sold": 18,
            "Products": "Vests",
            "Amount": 36
        },
        {
            "Date": new Date(2015,2,20),
            "Product_Categories": "Accessories",
            "Product_ID": 1002,
            "Sold": 24,
            "Products": "Cleaners",
            "Amount": 72
        },
        {
            "Date": new Date(2015,3,3),
            "Product_Categories": "Accessories",
            "Product_ID": 1001,
            "Sold": 12,
            "Products": "Bottles and Cages",
            "Amount": 24
        },
        {
            "Date": new Date(2015,0,18),
            "Product_Categories": "Accessories",
            "Product_ID": 1001,
            "Sold": 12,
            "Products": "Bottles and Cages",
            "Amount": 24
        },
        {
            "Date": new Date(2015,3,13),
            "Product_Categories": "Bikes",
            "Product_ID": 1005,
            "Sold": 6,
            "Products": "Road Bikes",
            "Amount": 450
        },
        {
            "Date": new Date(2015,9,1),
            "Product_Categories": "Bikes",
            "Product_ID": 1003,
            "Sold": 3,
            "Products": "Mountain Bikes",
            "Amount": 180
        },
        {
            "Date": new Date(2015,9,1),
            "Product_Categories": "Bikes",
            "Product_ID": 1004,
            "Sold": 3,
            "Products": "Mountain Bikes",
            "Amount": 180
        },
        {
            "Date": new Date(2015,9,2),
            "Product_Categories": "Clothings",
            "Product_ID": 1010,
            "Sold": 6,
            "Products": "Vests",
            "Amount": 12
        },
        {
            "Date": new Date(2015,9,21),
            "Product_Categories": "Clothings",
            "Product_ID": 1008,
            "Sold": 30,
            "Products": "Jerseys",
            "Amount": 150
        },
        {
            "Date": new Date(2015,9,12),
            "Product_Categories": "Clothings",
            "Product_ID": 1007,
            "Sold": 9,
            "Products": "Gloves",
            "Amount": 27
        },
        {
            "Date": new Date(2015,9,25),
            "Product_Categories": "Clothings",
            "Product_ID": 1007,
            "Sold": 6,
            "Products": "Gloves",
            "Amount": 18
        },
        {
            "Date": new Date(2015,9,29),
            "Product_Categories": "Clothings",
            "Product_ID": 1009,
            "Sold": 9,
            "Products": "Shorts",
            "Amount": 36
        },
        {
            "Date": new Date(2016,0,3),
            "Product_Categories": "Accessories",
            "Product_ID": 1002,
            "Sold": 20,
            "Products": "Cleaners",
            "Amount": 60
        },
        {
            "Date": new Date(2016,0,4),
            "Product_Categories": "Accessories",
            "Product_ID": 1001,
            "Sold": 16,
            "Products": "Bottles and Cages",
            "Amount": 32
        },
        {
            "Date": new Date(2016,0,5),
            "Product_Categories": "Accessories",
            "Product_ID": 1002,
            "Sold": 12,
            "Products": "Cleaners",
            "Amount": 36
        },
        {
            "Date": new Date(2016,0,8),
            "Product_Categories": "Accessories",
            "Product_ID": 1003,
            "Sold": 8,
            "Products": "Fenders",
            "Amount": 64
        },
        {
            "Date": new Date(2016,1,3),
            "Product_Categories": "Bikes",
            "Product_ID": 1004,
            "Sold": 4,
            "Products": "Mountain Bikes",
            "Amount": 240
        },
        {
            "Date": new Date(2016,0,4),
            "Product_Categories": "Bikes",
            "Product_ID": 1005,
            "Sold": 4,
            "Products": "Road Bikes",
            "Amount": 300
        },
        {
            "Date": new Date(2016,2,23),
            "Product_Categories": "Clothings",
            "Product_ID": 1010,
            "Sold": 12,
            "Products": "Vests",
            "Amount": 24
        },
        {
            "Date": new Date(2016,2,12),
            "Product_Categories": "Accessories",
            "Product_ID": 1001,
            "Sold": 8,
            "Products": "Bottles and Cages",
            "Amount": 16
        },
        {
            "Date": new Date(2016,2,19),
            "Product_Categories": "Accessories",
            "Product_ID": 1002,
            "Sold": 20,
            "Products": "Cleaners",
            "Amount": 60
        },
        {
            "Date": new Date(2016,2,20),
            "Product_Categories": "Accessories",
            "Product_ID": 1002,
            "Sold": 4,
            "Products": "Cleaners",
            "Amount": 12
        },
        {
            "Date": new Date(2016,2,19),
            "Product_Categories": "Bikes",
            "Product_ID": 1006,
            "Sold": 4,
            "Products": "Touring Bikes",
            "Amount": 260
        },
        {
            "Date": new Date(2015,3,1),
            "Product_Categories": "Bikes",
            "Product_ID": 1003,
            "Sold": 4,
            "Products": "Touring Bikes",
            "Amount": 260
        }
        ],
        rows: [{name: 'Products'}],
        columns: [{name:'Product_ID'}],
        values: [{name:'Amount'}, {name:'Sold', caption:'Units Sold'}],
        formatSettings: [{name:'Amount', format:'C1'}, {name:'Date',type:'date', format:'MM/dd/yyyy'}],
        groupSettings: [{ name: 'Products', type: 'Custom', 
                          customGroups:[{groupName:'Decors', items:['Cleaners','Fenders','Bottles and Cages']}]}]
      },
      height:'350px',
      width:'900px',
      showGroupingBar: true,
      allowGrouping : true
    };
  } ,
  provide:
  {
    pivotview:[GroupingBar, Grouping]
  }
}
</script>

<template>
  <ejs-pivotview :height="height" :width="width"
                 :dataSourceSettings="dataSourceSettings"
                 :showGroupingBar ="showGroupingBar"
                 :allowGrouping="allowGrouping"></ejs-pivotview>
</template>

<style >
  @import "../node_modules/@syncfusion/ej2-base/styles/bootstrap5.css";
  @import "../node_modules/@syncfusion/ej2-inputs/styles/bootstrap5.css";
  @import "../node_modules/@syncfusion/ej2-buttons/styles/bootstrap5.css";
  @import "../node_modules/@syncfusion/ej2-splitbuttons/styles/bootstrap5.css";
  @import "../node_modules/@syncfusion/ej2-calendars/styles/bootstrap5.css";
  @import "../node_modules/@syncfusion/ej2-dropdowns/styles/bootstrap5.css";
  @import "../node_modules/@syncfusion/ej2-lists/styles/bootstrap5.css";
  @import "../node_modules/@syncfusion/ej2-popups/styles/bootstrap5.css";
  @import "../node_modules/@syncfusion/ej2-navigations/styles/bootstrap5.css";
  @import "../node_modules/@syncfusion/ej2-grids/styles/bootstrap5.css";
  @import "../node_modules/@syncfusion/ej2-vue-pivotview/styles/bootstrap5.css";

 </style>


