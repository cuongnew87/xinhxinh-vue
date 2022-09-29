<template>
  <div>
    <div class="content">
      <Header />
      <Menu />
      <Body />
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Menu from "./components/Menu.vue";
import Body from "./components/Body.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "app",
  components: {
    Header,
    Menu,
    Body,
    Footer,
  },
};
</script>
