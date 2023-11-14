<template>
  <div id="app">
    <headerApp></headerApp>
    <topPage></topPage>
    <recordApp></recordApp>
    <columnApp></columnApp>
    <Footer />
  </div>
</template>

<script>
import TopPage from "./components/TopMyPage.vue";
import Header from "../src/components/Header.vue";
import Record from "./components/Record.vue";
import Column from "./components/Column.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",

  components: {
    topPage: TopPage,
    headerApp: Header,
    recordApp: Record,
    columnApp: Column,
    Footer,
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
#app {
  width: 1440px;
  padding: 0;
  margin: 0 auto;
}

.d-flex {
  display: flex;
}
</style>
