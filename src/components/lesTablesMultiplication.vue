<template>
  <div>
    <table class="table-multiplication" >
      <tbody>
        <div v-for="k in 10" v-bind:key="k">
         <table-multiplication v-bind:j="n" v-bind:i="k"/>
         </div>
      </tbody>
    </table>
    <br/>
  </div>
</template>

<script>
  import TableMultiplication from "./TableMultiplication.vue";

  export default {
    name: "TableMultiplication",
    props: {n: Number,
      },
    components: {
      TableMultiplication,
      
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
