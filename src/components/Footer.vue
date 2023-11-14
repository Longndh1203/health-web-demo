<template>
  <div class="footer">
    <div class="footer-container">
      <ul class="list-footers">
        <li
          v-for="(item, index) in dataFooters"
          :key="index"
          class="footer-item"
        >
          <p>{{ item.name }}</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProjectWebV1Footer",

  data() {
    return {
      dataFooters: [
        {
          name: "会員登録",
        },
        {
          name: "運営会社",
        },
        {
          name: "利用規約",
        },
        {
          name: "個人情報の取扱について",
        },
        {
          name: "特定商取引法に基づく表記",
        },
        {
          name: "お問い合わせ",
        },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.footer {
  padding: 0 80px;
  margin: 0 auto;
  width: 100%;
}

.footer-container {
  background: #414141;
  box-shadow: 0px 3px 6px 0px rgba(0, 0, 0, 0.16);
  display: flex;
  justify-content: space-between;
  margin: 0 auto;
  padding: 0 160px;
}

.list-footers {
  display: flex;
  height: 128px;
  align-items: center;
  justify-content: center;
  gap: 40px;
}

.list-footers p {
  color: #fff;
  font-family: Hiragino Kaku Gothic Pro;
  font-size: 11px;
  font-style: normal;
  font-weight: 300;
  line-height: 16px; /* 145.455% */
  letter-spacing: 0.033px;
}
</style>
