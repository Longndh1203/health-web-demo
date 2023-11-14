<template>
  <div class="home">
    <div class="home-top">
      <div class="hometop-gurupu-left">
        <img src="../assets/gurupu1.svg" alt="" />
      </div>
      <div class="home-top-gurupu-right"></div>
    </div>

    <list-hex />

    <!-- container -->
    <div class="home-container">
      <!-- list-foods -->
      <ListFoods />
      <button class="botan">記録をもっと見る</button>
    </div>
  </div>
</template>

<script>
import ListHex from "./ComponentLists/ListsHex/ListHex";
import ListFoods from "./ComponentLists/ListFoods/ListFoods.vue";
export default {
  name: "ProjectWebV1Home",
  components: {
    ListHex,
    ListFoods,
  },

  data() {
    return {};
  },

  mounted() {},

  methods: {},
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  list-style: none;
  text-decoration: none;
  border: none;
}

.home {
  min-height: 100vh;
  padding: 0 80px;
  margin: 0 auto;
  max-width: 100%;
}
.home-top {
  display: flex;
  width: 100%;
  margin: 0 auto;
  padding: 0;
}
.hometop-gurupu-left {
  display: flex;
}

.home-top-gurupu-right {
  width: 100%;
  background: #2e2e2e;
}

.home-container {
  margin: 0 atuo;
  padding: 20px 160px;
  width: 100%;
}

.botan {
  height: 56px;
  width: 296px;
  margin: 20px 332px;
  background: linear-gradient(33deg, #ffcc21 8.75%, #ff963c 86.64%);
  cursor: pointer;
  border: none;

  color: #fff;
  text-align: center;
  font-family: Hiragino Kaku Gothic Pro;
  font-size: 18px;
  font-style: normal;
  font-weight: 300;
  line-height: 26px; /* 144.444% */
}
</style>
