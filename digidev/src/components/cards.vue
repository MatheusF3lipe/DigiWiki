<template>
  <div class="Container">
    <div class="imagem">
      <img :src="Imagem" alt="" srcset="" />
    </div>
    <p>{{ nome }}</p>
  </div>
</template>

<style lang="scss" scoped>
.Container {
  width: 200px;
  border: 3px solid black;
  box-shadow: -1px 14px 31px 6px rgba(0, 0, 0, 0.9);
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>

<script>
export default {
  name: "card",
  props: {
    nome: String,
    Imagem: String,
  },
};
</script>
