<script>
export default {
  name: 'MainCard',
  props: ['name', 'race', 'img'],
};
</script>

<template>
  <div class="card">
    <div>
      <img :src="img" :alt="name" />
    </div>
    <div class="text">
      <h4>{{ name }}</h4>
      <p>{{ race }}</p>
    </div>
  </div>
</template>

<style scoped lang="scss">
.card {
  display: flex;
  flex-direction: column;
  width: calc(100% / 5);
  margin-bottom: 20px;
  text-align: center;

  .text {
    margin: 0 auto;
    font-size: 17px;
    font-family: Arial, Helvetica, sans-serif;

    h4 {
      margin: 10px;
    }
  }
}
</style>
