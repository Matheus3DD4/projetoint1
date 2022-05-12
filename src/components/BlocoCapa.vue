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
  <article class="blockcapa">
    <h2>{{ nome }}</h2>
    <h3>{{ ano }}</h3>
    <div class="imagem">
      <img :src="imagem" width="265" height="370" alt="" />
    </div>
  </article>
</template>
