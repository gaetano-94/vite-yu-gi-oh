<script>
export default {
  name: 'MainCard',
  props: ['name', 'type', 'img'],
};
</script>

<template>
  <div class="card">
    <div>
      <img :src="img" :alt="name" />
    </div>
    <div class="text">
      <h4>{{ name }}</h4>
      <h5>{{ type }}</h5>
    </div>
  </div>
</template>

<style scoped lang="scss">
@use '../assets/partial/variables.scss' as *;
.card {
  display: flex;
  flex-direction: column;
  width: calc(100% / 5 - 30px);
  margin-bottom: 20px;
  text-align: center;
  background-color: $bg-main;

  img {
    width: 100%;
  }

  .text {
    margin: 0 auto;
    font-size: 17px;
    font-family: Arial, Helvetica, sans-serif;
    margin-bottom: 40px;

    h4 {
      margin: 10px;
      color: white;
    }
  }
}
</style>
