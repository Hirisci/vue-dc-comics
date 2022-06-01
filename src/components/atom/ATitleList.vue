<template>
  <h4>{{ txt }}</h4>
</template>

<script>
export default {
  name: "ATitleList",
  props: ["txt"],
};
</script>

<style lang="scss" scoped>
h4 {
  font-weight: 600;
  text-transform: uppercase;
  margin: var(--margin-md) 0;
}
</style>