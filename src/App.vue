<template>
  <main class="flex flex-col text-center md:flex-row">
    <First_Header />
    <One_Form />
  </main>
</template>

<script>
import First_Header from './components/First_Header.vue';
import One_Form from './components/One_Form.vue';
import './assets/tailwind.css';

export default {
  name: 'App',

  components: {
    First_Header,
    One_Form
  }
}
</script>

<style lang="scss">
// Variaveis
$font-geral:'Poppins', sans-serif;

* {
  margin:0;
  padding: 0;
  box-sizing: border-box;
  font-size: 1rem;
  font-family: $font-geral;
}
body {
    background-image: url(../src/public/bg-intro-mobile.png);
    background-color: rgb(238, 78, 78);
    height: auto;
  }
</style>
