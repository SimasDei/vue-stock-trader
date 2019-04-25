<template>
  <div>
    <StockVue v-for="stock in stocks" :stock="stock" :key="stock.id"></StockVue>
  </div>
</template>
<script>
import StockVue from "./Stock.vue";
export default {
  data() {
    return {
      stocks: [
        { id: 1, name: "Mercedes", price: 110 },
        { id: 2, name: "Google", price: 200 },
        { id: 3, name: "Apple", price: 250 },
        { id: 4, name: "Twitter", price: 180 }
      ]
    };
  },
  components: {
    StockVue
  }
};
</script>
