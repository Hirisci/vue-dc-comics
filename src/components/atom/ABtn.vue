<template>
  <button>{{ text }}</button>
</template>

<script>
export default {
  nome: "ABtn",
  props: ["text"],
};
</script>


<style lang="scss" scoped>
button {
  background-color: transparent;
  border: transparent 2px solid;
}
</style>