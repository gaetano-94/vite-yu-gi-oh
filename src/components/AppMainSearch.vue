<script>
export default {
  name: 'MainSearch',
};
</script>

<template>
  <div class="container">
    <select name="searchcards" id="cards">
      <option selected="search">Search Cards</option>
      <option value="1">Spell Card</option>
      <option value="2">Trap Card</option>
      <option value="3">Normal Monster</option>
      <option value="4">Effect Monster</option>
      <option value="5">Flip Effect Monster</option>
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
