<script>
import axios from 'axios';
import AppMainCard from './AppMainCard.vue';
import AppMainFound from './AppMainFound.vue';

export default {
  name: 'MainCards',
  components: {
    AppMainCard,
    AppMainFound,
  },
  data() {
    return {
      cards: [],
      apiUrl: 'https://db.ygoprodeck.com/api/v7/cardinfo.php?num=40&offset=0',
    };
  },
  created() {
    axios.get(this.apiUrl).then((response) => {
      this.cards = response.data.data;
    });
  },
};
</script>

<template>
  <div class="container">
    <div class="container-cards">
      <div class="found">
        <AppMainFound :found="cards.length" />
      </div>
      <AppMainCard
        v-for="card in cards"
        :name="card.name"
        :type="card.type"
        :img="card.card_images[0].image_url"
      />
    </div>
  </div>
</template>

<style scoped lang="scss">
@use '../assets/partial/variables.scss' as *;
.container {
  width: 1140px;
  margin: 0 auto;
  background-color: white;
  padding: 50px 50px;

  .found {
    width: 100%;
    height: 60px;
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
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
}
</style>
