<template>
  <div class="mid-footer">
    <div class="container">
      <img src="/img/dc-logo-bg.png" alt="" />
      <MList :navList="footerFist" />
      <MList :navList="footerSec" />
      <MList :navList="footerTer" />
    </div>
  </div>
</template>

<script>
import MList from "../molecule/MList.vue";
export default {
  components: { MList },
  name: "OMidFooter",
  data() {
    return {
      footerFist: [
        {
          title: "dc comics",
          list: [
            "characters",
            "comics",
            "Movies",
            "tv",
            "games",
            "videos",
            "news",
          ],
        },
        {
          title: "shop",
          list: ["shop DC", "shop DC Collectionables"],
        },
      ],
      footerSec: [
        {
          title: "dc",
          list: [
            "terms of use",
            "Privacy Policy(new)",
            "ad Choices",
            "advertising",
            "jopbs",
            "subscriptions",
            "talent workshops",
            "CPSC Certificatee",
            "ratings",
            "shop help",
            "concats us",
          ],
        },
      ],
      footerTer: [
        {
          title: "Sites",
          list: [
            "DC",
            "MAD Magazine",
            "DC kids",
            "DC universe",
            "DC powe Visa",
          ],
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.mid-footer {
  background-image: url("../../../public/img/footer-bg.jpg");
  background-size: cover;

  .container {
    position: relative;
    color: #fff;
    display: flex;
    gap: 2.5rem;
    img {
      position: absolute;
      top: 0;
      right: 0;
      bottom: 0;
      height: 100%;
    }
  }
}
</style>