<template>
  <ul class="list-records">
    <li class="body-record" v-for="(item, index) in recordData" :key="index">
      <div class="body-record-content">
        <h4>{{ item.title }}</h4>
        <p>{{ item.name }}</p>
      </div>
    </li>
  </ul>
</template>

<script>
export default {
  name: "Health-Listrecords",

  data() {
    return {
      recordData: [
        {
          title: "BODY RECORD",
          name: "自分のカラダの記録",
        },
        {
          title: "MY EXERCISE",
          name: "自分の運動の記録",
        },
        {
          title: "MY DIARY",
          name: "自分の日記",
        },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.list-records {
  gap: 48px;
  display: flex;
}

.body-record {
  width: 288px;
  height: 288px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #ffcc21;
}

.body-record-content {
  gap: 8px;
  width: 240px;
  height: 244px;
  margin: auto;
  background-image: url("/src/assets/recommendBG.png");
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.body-record-content h4 {
  width: 240px;

  color: #ffcc21;
  text-align: center;
  font-family: Inter;
  font-size: 25px;
  font-style: normal;
  font-weight: 400;
  line-height: 30px; /* 120% */
  letter-spacing: 0.125px;
}
.body-record-content p {
  width: 160px;
  color: #fff;
  text-align: center;
  font-family: Hiragino Kaku Gothic Pro;
  font-size: 14px;
  font-style: normal;
  font-weight: 300;
  line-height: 20px; /* 142.857% */

  background: #ff963c;
}
</style>
