html
Copy code
<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
  data() {
    return {
      
    };
  },
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<template>
  <body>
    <Header></Header>
    <Main></Main>
    <Footer></Footer>
  </body>
</template>

<style lang="scss" scoped>

</style>