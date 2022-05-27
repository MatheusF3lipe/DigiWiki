<template>
  <div class="Container">
    <div class="imagem">
      <img :src="Imagem" alt="" srcset="" />
    </div>
    <p>{{ nome }}</p>
  </div>
</template>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css2?family=Luckiest+Guy&display=swap");
.Container {
  width: 200px;
  border: 5px solid black;
  box-shadow: 5px 5px 21px 5px #0000;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  p {
    margin-left: 30px;
    font-size: 18px;
    font-family: "Luckiest Guy", cursive;
  }
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
