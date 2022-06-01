<template>
  <div>
    <OTopFooter />
    <OMidFooter />
  </div>
</template>

<script>
import OMidFooter from "./OMidFooter.vue";
import OTopFooter from "./OTopFooter.vue";
export default {
  components: { OTopFooter, OMidFooter },
  name: "OFooter",
};
</script>

<style scope lang="scss">
</style>