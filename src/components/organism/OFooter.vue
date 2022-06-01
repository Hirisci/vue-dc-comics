<template>
  <footer>
    <OTopFooter />
    <OMidFooter />
    <OBotFooter />
  </footer>
</template>

<script>
import OBotFooter from "./OBotFooter.vue";
import OMidFooter from "./OMidFooter.vue";
import OTopFooter from "./OTopFooter.vue";
export default {
  components: { OTopFooter, OMidFooter, OBotFooter },
  name: "OFooter",
};
</script>

<style scope lang="scss">
</style>