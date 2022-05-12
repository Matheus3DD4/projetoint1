<script>
export default {
  // props: ["titulo"],
  props: {
    nome: {
      default: "A DEFINIR",
      type: String,
    },
    ano: String,
    imagem: String,
  },
};
</script>
<template>
  <article class="block">
    <h2>{{ nome }}</h2>
    <h3>{{ ano }}</h3>
    <div class="imagem">
      <img :src="imagem" width="175" height="270" alt="" />
    </div>
  </article>
</template>
