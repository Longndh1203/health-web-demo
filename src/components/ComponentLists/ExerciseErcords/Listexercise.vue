<template>
  <div class="exercise-record">
    <div class="exercise-record-container">
      <div class="title-exercise">
        <p>MY EXERCISE</p>
        <h3>2021.05.21</h3>
      </div>
      <ul class="list-exercise">
        <li
          class="exercise-content"
          v-for="(item, index) in exercises"
          :key="index"
        >
          <div class="exercise-name">
            <p>{{ item.title }}</p>
            <h5>{{ item.kalo }}</h5>
          </div>
          <h4>{{ item.time }}</h4>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProjectWebV1Listexercise",

  data() {
    return {
      exercises: [
        {
          title: "家事全般（立位・軽い）",
          kalo: "26kcal",
          time: "10 min",
        },
        {
          title: "家事全般（立位・軽い）",
          kalo: "26kcal",
          time: "10 min",
        },
        {
          title: "家事全般（立位・軽い）",
          kalo: "26kcal",
          time: "10 min",
        },
        {
          title: "家事全般（立位・軽い）",
          kalo: "26kcal",
          time: "10 min",
        },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.exercise-record {
  width: 960px;
  background: #414141;
  color: #fff;
}
.exercise-record-container {
  padding: 16px 24px;
}

.title-exercise {
  display: flex;
}

.title-exercise p {
  width: 96px;
  height: 36px;

  color: #fff;
  font-family: Inter;
  font-size: 15px;
  font-style: normal;
  font-weight: 400;
  line-height: 18px; /* 120% */
  letter-spacing: 0.15px;
}

.title-exercise h3 {
  width: 146px;

  color: #fff;
  font-family: Inter;
  font-size: 22px;
  font-style: normal;
  font-weight: 400;
  line-height: 27px; /* 122.727% */
  letter-spacing: 0.11px;
}

.list-exercise {
  padding-right: 32px;
  width: 880px;
  display: grid;
  grid-template-columns: auto auto;
  gap: 8px 40px;
}

.exercise-content {
  display: grid;
  grid-template-columns: auto auto;
  border-bottom: 1px solid #777;
}

.exercise-content h4 {
  color: #ffcc21;
  text-align: right;
  font-family: Inter;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 22px; /* 122.222% */
  letter-spacing: 0.09px;
}

.exercise-name h5 {
  color: #ffcc21;
  font-family: Inter;
  font-size: 15px;
  font-style: normal;
  font-weight: 400;
  line-height: 18px; /* 120% */
  letter-spacing: 0.075px;
}
</style>
