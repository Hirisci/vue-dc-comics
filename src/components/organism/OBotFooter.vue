<template>
  <div class="footer_bot">
    <div class="container">
      <ABtn class="btn -sing-up" :text="text" />
      <MSocialList :txt="follow" :socials="socials" />
    </div>
  </div>
</template>

<script>
import ABtn from "../atom/ABtn.vue";
import MSocialList from "../molecule/MSocialList.vue";
export default {
  components: { ABtn, MSocialList },
  name: "OBotFooter",
  data() {
    return {
      text: "sign-up now!",
      follow: "follow Us",
      socials: [
        { img: "footer-facebook.png", href: "#" },
        { img: "footer-twitter.png", href: "#" },
        { img: "footer-youtube.png", href: "#" },
        { img: "footer-pinterest.png", href: "#" },
        { img: "footer-periscope.png", href: "#" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.container {
  padding: var(--padding-lg);
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.footer_bot {
  background-color: var(--clr-bg-footer);
}

.-sing-up {
  border-color: var(--clr-active);
  color: #fff;
  text-transform: uppercase;
  font-size: 1rem;
  font-weight: 500;
  padding: var(--padding-md);
}
</style>