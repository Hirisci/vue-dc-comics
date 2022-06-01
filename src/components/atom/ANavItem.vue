<template>
  <li :class="{ active: isActive }">
    <a :href="href">{{ msg }}</a>
  </li>
</template>

<script>
export default {
  props: ["msg", "href", "isActive"],
  name: "ANavItem",
};
</script>

<style lang="scss" scoped>
li {
  a {
    padding: var(--padding-md);
    text-decoration: none;
    color: inherit;
    text-transform: uppercase;
    font-weight: 600;
    font-size: 0.8;
  }

  &.active {
    color: var(--clr-active);
  }

  &.active::after {
    content: "";
    display: inline;
    position: absolute;
    background-color: var(--clr-active);
    height: 0.3125rem;
  }

  &:hover {
    color: var(--clr-active);
  }
}
</style>