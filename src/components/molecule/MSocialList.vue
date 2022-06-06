<template>
  <div>
    <a-text class="social_title" :txt="txt" />
    <ul>
      <li v-for="(social, idx) in socials" :key="idx">
        <a :href="social.href"
          ><img :src="require(`@/assets/img/${social.img}`)" alt="social"
        /></a>
      </li>
    </ul>
  </div>
</template>

<script>
import AText from "../atom/AText.vue";
export default {
  components: { AText },
  props: ["txt", "socials"],
};
</script>

<style lang="scss" scoped>
div {
  display: flex;
  align-items: center;
  gap: 2rem;
}
ul {
  display: flex;
  align-items: center;
  gap: 0.75rem;
}
.social_title {
  text-transform: uppercase;
  font-weight: 800;
  font-size: 1.25rem;
  color: var(--clr-active);
}

a:hover img {
  transform: scale(1.2);
}
</style>