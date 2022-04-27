<template>
<main class="container-fluid">
  <JumboTron
    class="d-flex justify-content-center align-items-center text-center"
  />
 
  <FoodieJournal/>
  <PopularRecipes />
  <CucinaryCollection/>
  <FarmToTable/>
  <SubscribeComponent/>
  <CarouselComponent/>
  
  </main>
</template>

<script>
import JumboTron from "./JumboTron.vue";
import FoodieJournal from "@/components/FoodieJournal.vue";
import PopularRecipes from "./PopularRecipes.vue";
import CucinaryCollection from "./CucinaryCollection.vue";
import FarmToTable from "./FarmToTable.vue";
import SubscribeComponent from "./SubscribeComponent.vue"
import CarouselComponent from "./CarouselComponent.vue"

export default {
 
  name: "mainComp",
   components: {
    JumboTron,
    FoodieJournal,
    PopularRecipes,
    CucinaryCollection,
    FarmToTable,
    SubscribeComponent,
    CarouselComponent
  },
    
};
</script>

<style lang="scss" scoped>
main{
position: relative;
background-color: #f0eeeb;
}
</style>