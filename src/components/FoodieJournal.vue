<template>
  <div class="container ar-FJ">
    <div class="row">
      <h3 class="text-center text-uppercase mb-5">foodie journal</h3>
      <div class="d-flex">
        <CardComp
          v-for="(card, i) in cards"
          :key="i"
          :imgC="card.imgPos"
          :txtC="card.textPos"
          :idC="card.idPos"
          :monthC="card.monthPos"
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
      cards: [
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
          textPos: "Why These Toasts with Tea are My New Favorite",
          idPos: "By Emily Fields",
          monthPos: "March | 25th,2019",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.ar-FJ {
  position: absolute;
  top: 600px;
  right: 290px;
  background-color: white;
  padding: 35px;
}
</style>