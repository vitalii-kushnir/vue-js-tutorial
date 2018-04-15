<template>
    <div>
        <app-stock v-for="stock in stocks"></app-stock>
    </div>
</template>

<script>
  import Stock from './Stock.vue';

  export default {
    components: {
      appStock: Stock
    },

    data() {
      return {
        stocks : [
          {id:1, name: "bmw", price : 22 },
          {id:2, name: "audi", price : 33 },
          {id:3, name: "vw", price : 44 }
        ]
      }
    }
  }
</script>

<style>
</style>
