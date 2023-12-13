<script>
export default {
  name: 'MainSearch',

  data() {
    return {
      searchType: '',
    };
  },
};
</script>

<template>
  <div class="container">
    <select name="searchcards" id="cards" v-model="searchType">
      <option selected value="">Search Cards</option>
      <option value="Spell Card">Spell Card</option>
      <option value="Trap Card">Trap Card</option>
      <option value="Normal Monster">Normal Monster</option>
      <option value="Effect Monster">Effect Monster</option>
      <option value="Flip Effect Monster">Flip Effect Monster</option>
    </select>
  </div>
</template>

<style scoped lang="scss">
.container {
  width: 1140px;
  margin: 0 auto;

  select {
    font-size: 18px;
    margin: 20px 0px 20px 10px;
    width: 200px;
    padding: 5px;
    border-radius: 5px;
  }
}
</style>
