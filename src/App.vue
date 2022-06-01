<template>
  <div id="app">
    <OHeader />
    <OMain />
    <OFooter />
  </div>
</template>

<script>
import OFooter from "./components/organism/OFooter.vue";
import OMain from "./components/organism/OMain.vue";
import OHeader from "./components/organism/OHeader.vue";

export default {
  name: "App",
  components: {
    OHeader,
    OFooter,
    OMain,
  },
};
</script>

<style lang="scss">
@import "./assets/style/style.scss";

div > * {
  padding: var(--padding-md);
}
</style>
