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
  <article class="blockeditoras">
    <div class="h2">
      <h2>{{ nome }}</h2>
    </div>
    <div class="h3">
      <h3>{{ ano }}</h3>
    </div>
    <div class="imgedit">
      <img :src="imagem" width="178" height="275" alt="" />
    </div>
  </article>
</template>
