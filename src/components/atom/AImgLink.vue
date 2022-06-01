<template>
  <img :src="`/img/${src}`" :alt="name" />
</template>

<script>
export default {
  name: "AImgLink",
  props: ["src", "name"],
};
</script>

<style lang="scss" scoped>
img {
  height: 3.5rem;
}
</style>