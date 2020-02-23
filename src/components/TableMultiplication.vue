<template>
  <div>
    <h3>Table de 3</h3>
    <table class="table-multiplication" >
      <tbody>
         <TableRow v-bind:j="3" v-bind:i="1"/>
      </tbody>
    </table>
    <br/>
  </div>
</template>

<script>
  import TableRow from "./TableRow.vue";

  export default {
    name: "TableMultiplication",
    components: {
      TableRow
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
