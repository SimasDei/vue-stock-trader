<template>
  <div>
    <StockVue v-for="stock in stocks" :stock="stock" :key="stock.id"></StockVue>
  </div>
</template>
<script>
import StockVue from "./Stock.vue";

export default {
  components: {
    StockVue
  },
  computed: {
    stocks() {
      return this.$store.getters.stocks;
    }
  }
};
</script>
