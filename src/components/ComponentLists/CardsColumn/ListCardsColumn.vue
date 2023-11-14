<template>
  <ul class="list-cards-column">
    <li class="card-column" v-for="(item, index) in cards" :key="index">
      <div class="card-column-img">
        <p>{{ item.time }}</p>
      </div>
      <div class="card-column-text">
        <h6>{{ item.description }}</h6>
        <p>{{ item.attention }}</p>
      </div>
    </li>
  </ul>
</template>

<script>
export default {
  name: "ProjectWebV1ListCardsColumn",

  data() {
    return {
      cards: [
        {
          time: "2021.05.17   23:25",
          description:
            "魚を食べて頭もカラダも元気に！知っておきたい魚を食べるメリ… ",
          attention: "#魚料理  #和食  #DHA",
        },
        {
          time: "2021.05.17   23:25",
          description:
            "魚を食べて頭もカラダも元気に！知っておきたい魚を食べるメリ…",
          attention: "#魚料理  #和食  #DHA",
        },
        {
          time: "2021.05.17   23:25",
          description:
            "魚を食べて頭もカラダも元気に！知っておきたい魚を食べるメリ…",
          attention: "#魚料理  #和食  #DHA",
        },
        {
          time: "2021.05.17   23:25",
          description:
            "魚を食べて頭もカラダも元気に！知っておきたい魚を食べるメリ…",
          attention: "#魚料理  #和食  #DHA",
        },
        {
          time: "2021.05.17   23:25",
          description:
            "魚を食べて頭もカラダも元気に！知っておきたい魚を食べるメリ…",
          attention: "#魚料理  #和食  #DHA",
        },
        {
          time: "2021.05.17   23:25",
          description:
            "魚を食べて頭もカラダも元気に！知っておきたい魚を食べるメリ…",
          attention: "#魚料理  #和食  #DHA",
        },
        {
          time: "2021.05.17   23:25",
          description:
            "魚を食べて頭もカラダも元気に！知っておきたい魚を食べるメリ…",
          attention: "#魚料理  #和食  #DHA",
        },
        {
          time: "2021.05.17   23:25",
          description:
            "魚を食べて頭もカラダも元気に！知っておきたい魚を食べるメリ…",
          attention: "#魚料理  #和食  #DHA",
        },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.list-cards-column {
  padding-top: 20px;
  display: flex;
  gap: 8px;
  flex-wrap: wrap;
}

.card-column {
  width: 234px;
}

.card-column-img {
  background: url("/src/assets/cardColumnBG.png");
  height: 145px;
  display: flex;
  justify-content: flex-start;
  align-items: flex-end;
}

.card-column-img p {
  width: 144px;
  height: 24px;
  display: flex;
  justify-content: center;
  align-items: center;

  background: #ffcc21;

  color: #fff;
  font-family: Inter;
  font-size: 15px;
  font-style: normal;
  font-weight: 400;
  line-height: 30px; /* 200% */
}

.card-column-text {
  margin-top: 8px;
}

.card-column-text h6 {
  width: 232px;
  height: 48px;
  flex-shrink: 0;

  color: #414141;
  font-family: Hiragino Kaku Gothic Pro;
  font-size: 15px;
  font-style: normal;
  font-weight: 300;
  line-height: 22px; /* 146.667% */
  letter-spacing: 0.075px;
}

.card-column-text p {
  max-width: 232px;
  height: 24px;
  flex-shrink: 0;

  color: #ff963c;
  font-family: Hiragino Kaku Gothic Pro;
  font-size: 12px;
  font-style: normal;
  font-weight: 300;
  line-height: 22px; /* 183.333% */
  letter-spacing: 0.06px;
}
</style>
