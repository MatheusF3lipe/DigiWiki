<template>
  <div id="app">
    <topo lista="Digimon" class="cabeca"></topo>
    <div class="container">
      <cards
        class="card"
        v-for="(i, idx) in digimons"
        :key="idx"
        :nome="i.name"
        :Imagem="i.img"
      ></cards>
    </div>
  </div>
</template>

<script>
import api from "../services/api";
import cards from "./components/cards.vue";
import topo from "./components/topo.vue";

export default {
  name: "App",
  components: {
    topo,
    cards,
  },
  data() {
    return {
      digimons: [],
    };
  },
  methods: {},
  mounted() {
    api.get().then((response) => {
      this.digimons = response.data;
    });
  },
};
</script>

<style lang="scss">
@import "/assets/scss/geral.scss";
.container {
  max-width: 1220px;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  .card {
    margin-right: 150px;
    margin-bottom: 20px;
    margin-top: 50px;
  }
}
</style>
