<template>
  <header>
    <nav>
      <ul>
        <li>{{ lista }}</li>
        <li>{{ lista }}</li>
        <li>{{ lista }}</li>
      </ul>
    </nav>
  </header>
</template>
<script>
export default {
  name: "topo",
  props: {
    lista: String,
  },
};
</script>
<style lang="scss">
@import "../assets/scss/header.scss";
</style>


