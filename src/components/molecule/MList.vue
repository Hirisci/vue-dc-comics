<template>
  <div>
    <div v-for="(nav, idx) in navList" :key="idx">
      <ATitleList :txt="nav.title" />
      <ul>
        <li v-for="(li, indx) in nav.list" :key="indx">
          {{ li }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import ATitleList from "../atom/ATitleList.vue";
export default {
  components: { ATitleList },
  name: "MList",
  props: ["navList"],
};
</script>



<style lang="scss" scoped>
li {
  opacity: 0.5;
  text-transform: capitalize;
  font-size: 0.85rem;
  line-height: 1.2;
  margin-bottom: 0.25rem;
  cursor: pointer;
  &:hover {
    opacity: 1;
  }
}
</style>