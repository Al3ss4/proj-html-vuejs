<template>
  <div class="container food-jorn">
    <h3 class="text-center text-uppercase">foodie journal</h3>
    <CardComp />
  </div>
</template>

<script>
import CardComp from "./CardComp.vue";
export default {
  name: "FoodieJournal",
  components: {
    CardComp,
  },
};
</script>

<style>
</style>