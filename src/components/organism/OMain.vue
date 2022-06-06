<template>
  <main>
    <OSection class="hero"><AHeroImg /></OSection>
    <OSection> </OSection>
  </main>
</template>

<script>
import AHeroImg from "../atom/AHeroImg.vue";
// import OSection from "./OSection.vue";
export default {
  components: { AHeroImg },
  name: "OMain",
};
</script>

<style scoped lang="scss">
main {
  background-color: black;
  color: #fff;
}
</style>