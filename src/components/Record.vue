<template>
  <div class="record">
    <div class="record-container">
      <ListRecords />
      <div class="chart-record">
        <img src="../assets/bodyRecord.png" alt="" />
      </div>
      <ListexerciseVue />
      <ListDiariesVue />

      <button class="btn-records">記録をもっと見る</button>
    </div>
  </div>
</template>

<script>
import ListexerciseVue from "./ComponentLists/ExerciseErcords/Listexercise.vue";
import ListDiariesVue from "./ComponentLists/ListsDiaries/ListDiaries.vue";
import ListRecords from "./ComponentLists/ListsRecords/ListRecords.vue";

export default {
  name: "ProjectWebV1Record",
  components: {
    ListRecords,
    ListexerciseVue,
    ListDiariesVue,
  },

  data() {
    return {};
  },

  mounted() {},

  methods: {},
};
</script>

<style>
.record {
  width: 100%;
  padding: 20px 80px;
}
.record-container {
  margin: 0 auto;
  padding: 20px 160px;
  display: flex;
  flex-direction: column;
}

.chart-record {
  padding: 20px 0;
  width: 100%;
}

.chart-record img {
  width: 960px;
}

.btn-records {
  width: 296px;
  height: 56px;
  margin: 40px 312px;
  background: linear-gradient(33deg, #ffcc21 8.75%, #ff963c 86.64%);
}
</style>
