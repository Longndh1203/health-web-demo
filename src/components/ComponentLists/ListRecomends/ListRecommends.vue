<template>
  <ul class="list-recommends">
    <li class="recommend" v-for="(item, index) in recommends" :key="index">
      <h4>{{ item.title }}</h4>
      <p>{{ item.name }}</p>
    </li>
  </ul>
</template>

<script>
export default {
  name: "ProjectWebV1ListRecommends",

  data() {
    return {
      recommends: [
        { title: "RECOMMENDED COLUMN", name: "オススメ" },
        { title: "RECOMMENDED DIET", name: "ダイエット" },
        { title: "RECOMMENDED BEAUTY", name: "美容" },
        { title: "RECOMMENDED HEALTH", name: "健康" },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.list-recommends {
  display: flex;
  gap: 32px;
}

.recommend {
  width: 216px;
  height: 144px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background: url("/src/assets/recommendBG.png");
}

.recommend h4 {
  max-width: 200px;

  color: #ffcc21;
  text-align: center;
  font-family: Inter;
  font-size: 22px;
  font-style: normal;
  font-weight: 400;
  line-height: 27px; /* 122.727% */
  letter-spacing: 0.11px;
}

.recommend p {
  max-width: 200px;
  color: #fff;
  text-align: center;
  font-family: Hiragino Kaku Gothic Pro;
  font-size: 18px;
  font-style: normal;
  font-weight: 300;
  line-height: 26px; /* 144.444% */
}
</style>
