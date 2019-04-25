<template>
  <div>
    <h1>Trade of View your Portfolio</h1>
    <h6>You may Save & Load your Data</h6>
    <h6>Slick on 'End Day' to begin a new day of trading</h6>
    <p>Your Funds: {{ funds }}</p>
  </div>
</template>
<script>
export default {
  computed: {
    funds() {
      return this.$store.getters.funds;
    }
  }
};
</script>
