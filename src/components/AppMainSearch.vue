<script>
export default {
  name: 'MainSearch',
};
</script>

<template>
  <div class="container">
    <select name="type" id="">
      <option value="1">Spell Card</option>
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
