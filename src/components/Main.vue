<template>
<main class="container-fluid">
  <JumboTron
    class="d-flex justify-content-center align-items-center text-center"
  />
  <FoodieJournal />
  </main>
</template>

<script>
import JumboTron from "./JumboTron.vue";
import FoodieJournal from "@/components/FoodieJournal.vue";

export default {
 
  name: "mainComp",
   components: {
    JumboTron,
    FoodieJournal,
  },
};
</script>

<style lang="scss" scoped>
</style>