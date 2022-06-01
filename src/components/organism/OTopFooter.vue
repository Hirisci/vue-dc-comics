<template>
  <div class="footer-top">
    <div class="container">
      <m-footer-link
        v-for="(icon, idx) in navList"
        :src="icon.img"
        :name="icon.msg"
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
.footer-top {
  padding: var(--padding-xl) 0;
  background-color: var(--clr-active);
  .container {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    padding: var(--padding-md);
  }
}
</style>