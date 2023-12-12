<script>
export default {
  name: 'HeaderLogo',
};
</script>

<template>
  <div class="container-logo">
    <img src="../assets/img/logo.png" alt="Logo YU-GI-OH" />
    <h1>Yu-Gi-Oh Api</h1>
  </div>
</template>

<style scoped lang="scss">
.container-logo {
  width: 100%;
  height: 70px;
  display: flex;
  align-items: center;
  gap: 1.25rem;
  padding: 20px 20px;
  overflow: hidden;

  img {
    display: block;
    width: 100px;
    height: 100px;
    object-fit: cover;
  }

  h1 {
    font-size: 50px;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  }
}
</style>
