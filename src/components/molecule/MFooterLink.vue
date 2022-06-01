<template>
  <a href="#" class="card">
    <img :src="require(`@/asset/img/${src}`)" :alt="name" class="card_img" />
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
</style>