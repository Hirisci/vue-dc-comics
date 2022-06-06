<template>
  <div>
    <img :src="img" alt="" />
    <a-text :txt="text" />
  </div>
</template>

<script>
import AText from "../atom/AText.vue";
export default {
  components: { AText },
  props: {
    img: String,
    text: String,
  },
};
</script>

<style>
img {
  margin-bottom: 0.5rem;
}
</style>