<template>
  <main>
    <OSection class="hero" />
    <o-game-list />
  </main>
</template>

<script>
import OGameList from "./OGameList.vue";
import OSection from "./OSection.vue";

export default {
  components: { OSection, OGameList },
  name: "OMain",
};
</script>

<style scoped lang="scss">
main {
  background-color: var(--clr-bg-main);
  color: #fff;
}
</style>