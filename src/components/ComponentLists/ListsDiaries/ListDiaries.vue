<template>
  <div class="diary">
    <h2>MY DIARY</h2>
    <ul class="list-diaries">
      <li v-for="(item, index) in diaries" :key="index" class="diary-item">
        <h5>{{ item.time }}</h5>
        <h6>{{ item.title }}</h6>
        <p>{{ item.content }}</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "ProjectWebV1ListDiaries",

  data() {
    return {
      diaries: [
        {
          time: "2021.05.21   23:25",
          title: "私の日記の記録が一部表示されます。",
          content:
            "テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト…",
        },
        {
          time: "2021.05.21   23:25",
          title: "私の日記の記録が一部表示されます。",
          content:
            "テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト…",
        },
        {
          time: "2021.05.21   23:25",
          title: "私の日記の記録が一部表示されます。",
          content:
            "テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト…",
        },
        {
          time: "2021.05.21   23:25",
          title: "私の日記の記録が一部表示されます。",
          content:
            " テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト…",
        },
        {
          time: "2021.05.21   23:25",
          title: "私の日記の記録が一部表示されます。",
          content:
            "テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト…",
        },
        {
          time: "2021.05.21   23:25",
          title: "私の日記の記録が一部表示されます。",
          content:
            "テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト…",
        },
        {
          time: "2021.05.21   23:25",
          title: "私の日記の記録が一部表示されます。",
          content:
            "テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト…",
        },
        {
          time: "2021.05.21   23:25",
          title: "私の日記の記録が一部表示されます。",
          content:
            "テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト…",
        },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.diary {
  padding-top: 40px;
}

.list-diaries {
  display: grid;
  grid-template-columns: auto auto auto auto;
  gap: 8px;
}

.diary-item {
  border: 2px solid #707070;
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.diary-item h5 {
  margin: 8px 16px;
  color: #414141;
  font-family: Inter;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 22px; /* 122.222% */
  letter-spacing: 0.09px;
  width: 147px;
}

.diary-item h6 {
  margin: 0 16px;
  color: #414141;
  font-family: Inter;
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: 22px; /* 122.222% */
  letter-spacing: 0.09px;
}

.diary-item p {
  margin: 4px 16px;

  color: #414141;
  font-family: Hiragino Kaku Gothic Pro;
  font-size: 12px;
  font-style: normal;
  font-weight: 300;
  line-height: 17px; /* 141.667% */
  letter-spacing: 0.06px;
}
</style>
