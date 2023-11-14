<template>
  <ul class="list-foods">
    <li v-for="(item, index) in foods" :key="index">
      <a href="">
        <div class="food-card">
          <button>
            <p>{{ item.time }}</p>
          </button>
        </div>
      </a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "ProjectWebV1ListFoods",

  data() {
    return {
      foods: [
        {
          time: "05.21.Morning",
        },
        {
          time: "05.21.Lunch",
        },
        {
          time: "05.21.Dinner",
        },
        {
          time: "05.21.Snack",
        },
        {
          time: "05.20.Morning",
        },
        {
          time: "05.20.Lunch",
        },
        {
          time: "05.20.Dinner",
        },
        {
          time: "05.21.Snack",
        },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.list-foods {
  display: flex;
  gap: 8px;
  display: flex;
  flex-wrap: wrap;
}

.food-card {
  display: flex;
  width: 234px;
  height: 234px;
  justify-content: flex-start;
  align-items: end;
  background: url("/src/assets/list-foods/food1.png");
}

.food-card button {
  width: 120px;
  height: 32px;
  text-align: center;
  display: flex;
  justify-content: center;
  background: #ffcc21;
}

.food-card p {
  margin: auto;
  color: #fff;
  font-family: Inter;
  font-size: 15px;
  font-style: normal;
  font-weight: 400;
  line-height: 18px; /* 120% */
  letter-spacing: 0.15px;
}
</style>
