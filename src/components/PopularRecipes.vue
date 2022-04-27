<template>
  <div class="container ar-PR">
    <div class="row">
      <h4 class="text-center text-uppercase">popular recipies</h4>
      <p class="text-center fst-italic mt-3 grey">
        Aliquam erat volutpat. Ut quis ligula a magna blandit
        finibus.Suspendisse
      </p>
      <p class="text-center fst-italic grey">
        lacus non nunc lacinia lobortis.
      </p>
      <div class="col-6 p-r-poster">
        <CardPopularRecipes
          v-for="(cardR, i) in cardsR"
          :key="i"
          :imgCR="cardR.imgCR"
          :ttlCR="cardR.ttlCR"
          :idCR="cardR.idCR"
          :txtCR="cardR.textCR"
        />
      </div>
      <div class="col-6 p-r-poster">
        <PosterPopularRecipes
          v-for="(poster, i) in posters"
          :key="i"
          :imgPR="poster.imgP"
        />
      </div>
    </div>
  </div>
</template>

<script>
import CardPopularRecipes from "./CardPopularRecipes.vue";
import PosterPopularRecipes from "./PosterPopularRecipes.vue";
export default {
  name: "popularRecipes",
  components: {
    CardPopularRecipes,
    PosterPopularRecipes,
  },
  data() {
    return {
      posters: [
        {
          imgP: "Mixed-fruits-460x295",
        },
        {
          imgP: "r-rachel-park-366508-unsplash-min-460x295",
        },
        {
          imgP: "r-michelle-tsang-500721-unsplash-min-460x295",
        },
        {
          imgP: "quick-summer-drink-460x295",
        },
        {
          imgP: "r-maarten-van-den-heuvel-400626-unsplash-min-460x295",
        },
        {
          imgP: "perfect-cosmopolitan-460x295",
        },
        {
          imgP: "fi2x-6-460x295",
        },
        {
          imgP: "r-brooke-lark-96398-unsplash-min-460x295",
        },
      ],
      cardsR: [
        {
          imgCR: "Mixed-fruits-460x295",
          ttlCR: "Lunch Favourite With Salad, Naan And Beans",
          idCR: "Bakery, Featured, Healthy, Latest Recipes, Staff Picks",
          textCR:
            "Suspendisse at semper odio. Nam fringilla scelerisque tincidunt. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec tincidunt posuere ornare, Phasellus placerat odionon feugiat sollicitudin. Integer vitae elementum ex. Sed porttitor, diam eget convallis volutpat, arcu tellus facilisis nulla, id dignissim orci leo id",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.ar-PR {
  margin-top: 450px;
  .grey {
    color: grey;
  }
}
.p-r-poster {
  margin-top: 60px;
}
</style>