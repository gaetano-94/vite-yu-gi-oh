<script>
import AppHeaderLogo from './AppHeaderLogo.vue';
export default {
  name: 'Header',
  components: {
    AppHeaderLogo,
  },
};
</script>

<template>
  <header class="container">
    <AppHeaderLogo />
  </header>
</template>

<style scoped lang="scss">
.container {
  width: 100%;
}
</style>
