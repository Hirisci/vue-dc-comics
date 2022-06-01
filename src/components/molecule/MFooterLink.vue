<template>
  <a href="#" class="card">
    <img :src="`/img/${src}`" :alt="name" class="card_img" />
    <div class="card_name">{{ name }}</div>
  </a>
</template>

<script>
export default {
  name: "MFooterCard",
  props: ["src", "name"],
};
</script>

<style lang="scss" scoped>
.card {
  img {
    width: 50px;
    aspect-ratio: 1/1;
  }
}
</style>