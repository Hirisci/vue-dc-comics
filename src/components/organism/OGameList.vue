<template>
  <section class="container">
    <a-btn class="btn-main -big" text="Current series" />

    <div class="gallery">
      <m-game-item
        v-for="(game, idx) in database"
        :key="idx"
        :img="game.thumb"
        :text="game.series"
      />
    </div>

    <a-btn class="btn-main" text="Load More" />
  </section>
</template>

<script>
import Jdata from "../../assets/data/dc-comics.json";
import ABtn from "../atom/ABtn.vue";
import MGameItem from "../molecule/MGameItem.vue";

export default {
  components: { ABtn, MGameItem },
  name: "OGameList",
  data: function () {
    return {
      database: Jdata,
    };
  },
};
</script>

<style lang="scss" scoped>
section {
  position: relative;

  text-align: center;

  button:last-child {
    margin-bottom: 1.5rem;
  }
}

.gallery {
  padding-top: 2rem;
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  gap: 1.5rem;
  padding-bottom: 1.5rem;
}
</style>