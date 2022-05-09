<script>
import NovoBloco from "./NovoBloco.vue";
export default {
  components: { NovoBloco },
  data() {
    return {
      editoras: [
        {
          nome: "Antofágica",
          ano: "04/2022",
          imagem: new URL("./img/antofagica.jpg", import.meta.url).href,
        },
        {
          nome: "Buzz",
          ano: "02/2021",
          imagem: new URL("./img/buzz.jpg", import.meta.url).href,
        },
        {
          nome: "Amoler",
          ano: "02/2021",
          imagem: new URL("./img/amoler.jpg", import.meta.url).href,
        },
        {
          nome: "Biblioteca Azul",
          ano: "2021",
          imagem: new URL("./img/biblue.jpg", import.meta.url).href,
        },
        {
          nome: "Companhia das Letras",
          ano: "2021",
          imagem: new URL("./img/complet.jpg", import.meta.url).href,
        },
        {
          nome: "Aleph",
          ano: "2021",
          imagem: new URL("./img/aleph.jpg", import.meta.url).href,
        },
      ],
      imagens: [
        {
          nome: "Original",
          ano: "2009",
          imagem: new URL("./img/original.jpeg", import.meta.url).href,
        },
      ],
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
    <NovoBloco
      v-for="(editora, i) of editoras"
      :key="i"
      :nome="editora.nome"
      :ano="editora.ano"
      :imagem="editora.imagem"
    />
  </section>
</template>
<style></style>
