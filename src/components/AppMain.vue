<script>
import AppMainSearch from './AppMainSearch.vue';
import AppMainCards from './AppMainCards.vue';

export default {
  name: 'Main',
  components: {
    AppMainSearch,
    AppMainCards,
  },
};
</script>

<template>
  <main>
    <AppMainSearch />
    <AppMainCards />
  </main>
</template>

<style scoped lang="scss"></style>
