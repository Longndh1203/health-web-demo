<template>
  <ul style="display: flex" class="home-listMenu">
    <li v-for="(item, index) in arrayHex" :key="index">
      <a href="">
        <div class="home-hex">
          <img src="../../../assets/list-hexs/icon_knife.png" alt="" />
          <p>{{ item.session }}</p>
        </div>
      </a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "ListHex",

  data() {
    return {
      arrayHex: [
        {
          session: "Morning",
          url: "/public/listHexs/icon_knife.png",
        },
        {
          session: "Lunch",
          url: "/public/listHexs/icon_knife.png",
        },
        {
          session: "Dinner",
          url: "/public/listHexs/icon_knife.png",
        },
        {
          session: "Snack",
          url: "/public/listHexs/icon_knife.png",
        },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.home-listMenu {
  padding: 20px 272px;
  display: flex;
  justify-content: space-around;
}

.home-hex {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 116px;
  height: 134px;
  gap: 8px;
  background: url(../../../assets/list-hexs/hexBG.png);
}
.home-hex p {
  color: #fff;
  text-align: center;
  font-family: Inter;
  font-size: 20px;
  font-style: normal;
  font-weight: 400;
  line-height: 24px; /* 120% */
}
</style>
