<template>
  <div class="Column">
    <div class="Column-container">
      <!-- listRecommend -->
      <ListRecommends />

      <ListCardsColumn />

      <button class="botan">記録をもっと見る</button>
    </div>
  </div>
</template>

<script>
import ListCardsColumn from "./ComponentLists/CardsColumn/ListCardsColumn.vue";
import ListRecommends from "./ComponentLists/ListRecomends/ListRecommends.vue";

export default {
  name: "ProjectWebV1Column",
  components: {
    ListRecommends,
    ListCardsColumn,
  },

  data() {
    return {};
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.Column {
  width: 100%;
  padding: 20px 80px;
}

.Column-container {
  margin: 0 auto;
  padding: 20px 160px;
}
</style>
