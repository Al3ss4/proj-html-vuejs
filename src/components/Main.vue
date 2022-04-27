<template>
<main class="container-fluid">
  <JumboTron
    class="d-flex justify-content-center align-items-center text-center"
  />
 
  <FoodieJournal/>
  <PopularRecipes />
  <CucinaryCollection/>
  <FarmToTable/>
  </main>
</template>

<script>
import JumboTron from "./JumboTron.vue";
import FoodieJournal from "@/components/FoodieJournal.vue";
import PopularRecipes from "./PopularRecipes.vue";
import CucinaryCollection from "./CucinaryCollection.vue";
import FarmToTable from "./FarmToTable.vue"

export default {
 
  name: "mainComp",
   components: {
    JumboTron,
    FoodieJournal,
    PopularRecipes,
    CucinaryCollection,
    FarmToTable
  },
    
};
</script>

<style lang="scss" scoped>
main{
position: relative;
background-color: #f0eeeb;
}
</style>