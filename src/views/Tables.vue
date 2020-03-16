<template>
  <div>
    <h2>Les tables de multiplications</h2>
      <div v-for="k in 10" v-bind:key="k">
        <les-tables-multiplication v-bind:n="k"/>
      </div>
      <hr/>
  </div>
</template>

<script>
  import lesTablesMultiplication from "../components/TableMultiplication.vue";

  export default {
    name: "home",
    data: function () {
      return {
        n: 8
      };
    },
    name: "TableMultiplication",
    components: {
      lesTablesMultiplication,
      
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .table-multiplication {
    text-align: center;
    margin-left: auto;
    margin-right: auto;
    background-color: lightblue;
  }
</style>