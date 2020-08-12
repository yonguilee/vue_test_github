<template>
  <v-container>
    <grid :data="gridProps.data" :columns="gridProps.columns" />
  </v-container>
</template>

<script>
import "tui-grid/dist/tui-grid.css";
import { Grid } from "@toast-ui/vue-grid";

export default {
  name: "GridTypeA",
  components: {
    grid: Grid
  },
  data: () => ({}),
  created() {
    this.gridProps = {
      data: [
        // for rowData prop
        {
          th1: "1",
          th2: "th5",
          th3: "PO1",
          th4: "th5",
          th5: "checked",
          th6: "th5",
          th7: "Y",
          th8: "th5th5",
          th9: "th5th5th5th5",
          th10: "2020-01-01",
          th11: "9999-12-31",
          th12: ""
        },
        {
          th1: "2",
          th2: "th5th5",
          th3: "PO1",
          th4: "th5",
          th5: "checked",
          th6: "th5",
          th7: "Y",
          th8: "th5th5",
          th9: "th5th5th5th5",
          th10: "2020-01-01",
          th11: "9999-12-31",
          th12: ""
        }
      ],
      columns: [
        // for columnData prop
        {
          header: "No",
          name: "th1"
        },
        {
          header: "asdasd",
          name: "th2"
        },
        {
          header: "dasd항asdasd",
          name: "th3"
        },
        {
          header: "asdasfasf",
          name: "th4"
        },
        {
          header: "th5",
          name: "th5"
        },
        {
          header: "th5",
          name: "th6"
        },
        {
          header: "th5",
          name: "th7"
        },
        {
          header: "th5",
          name: "th8"
        },
        {
          header: "th5",
          name: "th9"
        },
        {
          header: "th5",
          name: "th10"
        },
        {
          header: "종료일자",
          name: "th11"
        },
        {
          header: "비고",
          name: "th12"
        }
      ]
    };
  }
};
</script>
