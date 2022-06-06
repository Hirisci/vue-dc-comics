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
.btn-main {
  background-color: var(--clr-active);
  color: var(--clr-text-1);
  text-transform: uppercase;
  font-weight: 600;
  padding: var(--padding-xs) var(--padding-md);

  &.-big {
    font-size: 1.2rem;
    position: absolute;
    left: 0;
    top: 0;
    transform: translateY(-50%);
  }
}
</style>