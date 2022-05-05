<script>
import NovoBloco from "./NovoBloco.vue";
export default {
  components: { NovoBloco },
  data() {
    return {
      nome: ["2012"],
    };
  },
};
</script>
<template>
  <section id="capa">
    <NovoBloco titulo="Companhia das Letras" :nome="['07/2009']" />
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
<style>
</style>
