
<template>
  <header class="container">
    <a-logo />
    <m-nav />
  </header>
</template>

<script>
import ALogo from "../atom/ALogo.vue";
import MNav from "../molecule/MNav.vue";

export default {
  components: { ALogo, MNav },
  name: "OHeader",
};
</script>

<style scoped lang="scss">
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: relative;
}
</style>