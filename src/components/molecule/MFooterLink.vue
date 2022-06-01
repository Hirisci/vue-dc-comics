<template>
  <a href="#" class="card">
    <AImgLink :src="src" :name="name" class="card_img" />
    <AText :txt="name" class="card_name" />
  </a>
</template>

<script>
import AImgLink from "../atom/AImgLink.vue";
import AText from "../atom/AText.vue";
export default {
  components: { AImgLink, AText },
  name: "MFooterCard",
  props: ["src", "name"],
};
</script>

<style lang="scss" scoped>
.card {
  display: flex;
  flex-direction: row;
  align-items: center;
  text-decoration: none;
  color: var(--clr-text-1);
  gap: 0.5rem;

  &_name {
    text-transform: uppercase;
  }
}

.card:last-of-type {
  img {
    height: 2.5rem;
  }
}
</style>