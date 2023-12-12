<script>
export default {
  name: 'MainSearch',
};
</script>

<template>
  <div class="container">
    <select name="Alien" id="">
      <option value="1">Alien</option>
    </select>
  </div>
</template>

<style scoped lang="scss">
.container {
  width: 1140px;
  margin: 0 auto;

  select {
    font-size: 18px;
    margin-top: 20px;
    margin-left: 30px;
    width: 200px;
    padding: 5px;
    border-radius: 5px;
  }
}
</style>
