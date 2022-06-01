<template>
  <div class="footer-top">
    <div class="container">
      <m-footer-link
        v-for="(icon, idx) in navList"
        :src="incon.img"
        :name="icon.name"
        :key="idx"
      />
    </div>
  </div>
</template>

<script>
import MFooterLink from "../molecule/MFooterLink.vue";
export default {
  components: { MFooterLink },
  name: "OFooterTop",
  data() {
    return {
      navList: [
        {
          msg: "digital comics",
          img: "buy-comics-digital-comics.png",
        },
        {
          msg: "dc merchandise",
          img: "buy-comics-merchandise.png",
        },
        {
          msg: "subscription",
          img: "buy-comics-subscriptions.png",
        },
        {
          msg: "comic shop locator",
          img: "buy-comics-shop-locator.png",
        },
        {
          msg: "dc power visa",
          img: "buy-dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.footer__top {
  background-color: var(--clr-active);
  height: 20rem;
}
</style>