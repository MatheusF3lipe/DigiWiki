<template>
  <div id="app">
    <topo lista="Digimon"></topo>
  </div>
</template>

<script>
import topo from "./components/topo.vue";

export default {
  name: "App",
  components: {
    topo,
  },
};
</script>

<style lang="scss">
@import "/assets/scss/geral.scss";
</style>
