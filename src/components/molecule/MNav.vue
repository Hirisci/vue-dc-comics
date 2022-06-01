<template>
  <nav>
    <ul>
      <a-nav-item
        v-for="(item, idx) in navList"
        :key="idx"
        :msg="item.msg"
        :isActive="item.isActive"
        :href="item.href"
      />
    </ul>
  </nav>
</template>

<script>
import ANavItem from "../atom/ANavItem.vue";
export default {
  data() {
    return {
      navList: [
        {
          msg: "characters",
          href: "#",
          isActive: false,
        },
        {
          msg: "comics",
          href: "#",
          isActive: true,
        },
        {
          msg: "movies",
          href: "#",
          isActive: false,
        },
        {
          msg: "tv",
          href: "#",
          isActive: false,
        },
        {
          msg: "games",
          href: "#",
          isActive: false,
        },
        {
          msg: "collectibles",
          href: "#",
          isActive: false,
        },
        {
          msg: "videos",
          href: "#",
          isActive: false,
        },
        {
          msg: "fans",
          href: "#",
          isActive: false,
        },
        {
          msg: "news",
          href: "#",
          isActive: false,
        },
        {
          msg: "shop",
          href: "#",
          isActive: false,
        },
      ],
    };
  },
  components: { ANavItem },
  name: "MNav",
};
</script>

<style lang="scss" scoped>
ul {
  display: flex;
}
</style>>