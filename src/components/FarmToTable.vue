<template>
  <div class="container">
    <div class="row ms-3">
      <div class="d-flexjustify-content-start col-6">
        <h4 class="text-uppercase mt-5">farm to table</h4>
        <p class="fst-italic mt-3 grey">
          Aliquam erat volutpat. Ut quis ligula a magna blandit
          finibus.Suspendisse
        </p>
        <p class="fst-italic">maximus lacus non nunc lacinia lobortis.</p>
      </div>
      <div class="col-6 d-flex justify-content-end">
        <button type="button" class="btn btn-orange text-uppercase mt-5">
          read our blog
          <span><i class="fa-solid fa-book-open-reader mx-1"></i> </span>
        </button>
      </div>
    </div>
    <div class="row">
      <div class="col-8">
        <CardSXFarm
          v-for="(item, i) in items"
          :key="i"
          :imgSX="item.imgCardSX"
          :ttlSX="item.ttlCardSX"
          :idSX="item.idCardSX"
          :dateSX="item.dateCardSX"
          :txtSX="item.textCardSX"
        />
        <div>
          <CardCollectionSX
            v-for="(element, i) in elements"
            :key="i"
            :imgCCSX="element.imgCSX"
            :txtCCSX="element.textCSX"
            :idCCSX="element.idCSX"
            :monthCCSX="element.monthCSX"
            class="mt-5"
          />
        </div>
      </div>
      <div class="col-4">
        <CardDXFarm  v-for="(poster, i) in posters" :key="i" :imgDX="poster.imgDX"/>
      </div>
    </div>
  </div>
</template>

<script>
import CardSXFarm from "./CardSXFarm.vue";
import CardDXFarm from "./CardDXFarm.vue";
import CardCollectionSX from "./CardCollectionSX.vue";
export default {
  name: "farmToTable",
  components: {
    CardSXFarm,
    CardDXFarm,
    CardCollectionSX,
  },
  data() {
    return {
      items: [
        {
          imgCardSX: "single-post-img3-600x395",
          ttlCardSX: "Food Corner: Top Japanese Restaurants for Sushi",
          idCardSX: "By admin",
          dateCardSX: "March | 25th,2019",
          textCardSX:
            "Suspendisse at semper odio. Nam fringilla scelerisque tincidunt. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec tincidunt posuere ornare, Phasellus placerat odio non feugiat sollicitudin. Integer vitae elementum ex.",
        },
      ],
      elements: [
        {
          imgCSX: "fi-roundup-200x132",
          textCSX: "Roundup: My New Favourite Recipes For Healthy Living",
          idCSX: "By Emily Fields",
          monthCSX: "March | 25th,2019",
        },
        {
          imgCSX: "fi-korean-food-200x132",
          textCSX: "Meal Prep: Korean Bibimbap with Kimchi",
          idCSX: "By Emily Fields",
          monthCSX: "March | 25th,2019",
        },
        {
          imgCSX: "fi-toasts-200x132",
          textCSX: "Why These Toasts with Tea are My New Favorite",
          idCSX: "By admin",
          monthCSX: "March | 25th,2019",
        },
        {
          imgCSX: "fi-street-food-200x132",
          textCSX: "Exploring Street Food in Bangkok",
          idCSX: "By admin",
          monthCSX: "March | 25th,2019",
        },

        {
          imgCSX: "fi-organic-breakfast-200x132",
          textCSX: "Organic Choices For Healthier Living",
          idCSX: "By Emily Fields",
          monthCSX: "March | 25th,2019",
        },
        {
          imgCSX: "fi-water-side-rest-200x132",
          textCSX: "5 Waterside Restaurants in Istanbul for Special Events",
          idCSX: "By Emily Fields",
          monthCSX: "March | 25th,2019",
        },
      ],
      posters:[
          {
              imgDX:"ad-bg",
          }
      ]
    };
  },
};
</script>

<style lang="scss" scoped>
.btn-orange {
  background-color: orangered;
  border-radius: 0rem;
  color: white;
  width: 200px;
  height: 50px;
}
</style>