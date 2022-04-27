<template>
  <div class="container ar">
    <div class="row">
      <h3 class="text-center text-uppercase mb-5">foodie journal</h3>
      <div class="d-flex">
        <CardComp
          v-for="(poster, i) in posters"
          :key="i"
          :imgC="poster.imgPos"
          :txtC="poster.textPos"
          :idC="poster.idPos"
          :monthC="poster.monthPos"
        />
      </div>
    </div>
  </div>
</template>

<script>
import CardComp from "./CardComp.vue";
export default {
  name: "FoodieJournal",
  components: {
    CardComp,
  },
  data() {
    return {
      posters: [
        {
          imgPos: "single-post-img3-200x132",
          textPos: "Food Corner: Top Japanese Restaurants for Sushi",
          idPos: "By admin",
          monthPos: "March | 25th,2019",
        },
        {
          imgPos: "fi-roundup-200x132",
          textPos: "Roundup: My New Favourite Recipes For Healthy Living",
          idPos: "By Emily Fields",
          monthPos: "March | 25th,2019",
        },
        {
          imgPos: "fi-toasts-200x132",
          textPos: "Wht These Toasts with Tea are My New Favorite",
          idPos: "By Emily Fields",
          monthPos: "March | 25th,2019",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.ar {
  position: absolute;
  top: 600px;
  right: 290px;
  background-color: white;
  padding: 35px;
}
</style>