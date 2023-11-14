<template>
  <div class="header">
    <div class="header-container">
      <div class="header-logo">
        <img src="../assets/logo.png" alt="" />
      </div>
      <div class="header-navbar" style="display: flex">
        <ul style="display: flex; gap: 24px">
          <li class="header-memo">
            <a href=""
              ><img src="../assets/memo.svg" alt="" />
              <p>自分の記録</p>
            </a>
          </li>
          <li class="header-challenge">
            <a href=""
              ><img src="../assets/challenge.svg" alt="" />
              <p>チャレンジ</p>
            </a>
          </li>
          <li class="header-info">
            <a href=""
              ><img src="../assets/info.svg" alt="" />
              <p>お知らせ</p>
            </a>
          </li>
        </ul>
        <img src="../assets/menu.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProjectWebV1Header",

  data() {
    return {};
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  list-style: none;
}

.header {
  padding: 0 80px;
  margin: 0 auto;
  width: 100%;
}

.header-container {
  background: #414141;
  box-shadow: 0px 3px 6px 0px rgba(0, 0, 0, 0.16);
  display: flex;
  justify-content: space-between;
  margin: 0 auto;
  padding: 0 160px;
}

.header-logo {
  padding: 8px 0;
}

.header-navbar {
  padding: 8px 0;
}
.header-navbar ul li {
  margin: 8px;
}

.header-navbar ul li a {
  display: flex;
  gap: 8px;
}

.header-navbar ul li a img {
  width: 32px;
  height: 32px;
}

.header-navbar ul li a p {
  width: 96px;
  color: #fff;
  font-family: Hiragino Kaku Gothic Pro;
  font-size: 16px;
  font-style: normal;
  font-weight: 300;
  line-height: 23px;
  margin: auto;
}
</style>
