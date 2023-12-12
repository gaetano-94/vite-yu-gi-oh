<script>
export default {
  name: 'MainCards',
};
</script>

<template>
  <div class="container">
    <div class="found">
      <h3>Found 39 cards</h3>
    </div>
    <div class="container-cards">
      <div class="card"></div>
    </div>
  </div>
</template>

<style scoped lang="scss">
@use '../assets/partial/variables.scss' as *;
.container {
  width: 1140px;
  height: 100%;
  margin: 0 auto;
  background-color: aqua;
  padding: 50px 50px;

  .found {
    width: 100%;
    height: 50px;
    background-color: $bg-found;
    display: flex;
    align-items: center;

    h3 {
      color: white;
      margin-left: 20px;
    }
  }

  .container-cards {
    width: 100%;
    background-color: yellow;
    height: 1000px;
  }
}
</style>
