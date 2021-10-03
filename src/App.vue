<template>
  <NavBar />
  <router-view />
  <Footer />
</template>
<script>
import NavBar from "./components/NavBar";
import Footer from "./components/Footer";
export default {
  components: {
    NavBar,
    Footer,
  },
};
</script>
<style>
</style>
