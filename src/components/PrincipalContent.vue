<script>
import NovoBloco from "./NovoBloco.vue";
export default {
  components: { NovoBloco },
  data() {
    return {
      imagens: [new URL("./img/original.jpeg", import.meta.url).href],
    };
  },
};
</script>
<template>
  <section id="capa">
    <section v-for="(imagem, i) of imagens" :key="i">
      <img :src="imagem" alt="" />
    </section>
  </section>
  <section id="editoras">
    <NovoBloco titulo="Antofágica" :nome="['04/2022']" />
    <NovoBloco titulo="Buzz" :nome="['02/2021']" />
    <NovoBloco titulo="Aleph" :nome="['2021']" />
    <NovoBloco titulo="Biblioteca Azul" :nome="['2021']" />
    <NovoBloco titulo="Companhia das Letras" :nome="['2021']" />
    <NovoBloco titulo="Amoler" :nome="['02/2021']" />
    <NovoBloco />
  </section>
</template>
<style></style>
