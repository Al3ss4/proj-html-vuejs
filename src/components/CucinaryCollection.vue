<template>
  <div class="container">
    <div class="row">
           <h4 class="text-center text-uppercase cucinary-collection">cucinary collection</h4>
      <p class="text-center fst-italic mt-3 grey">
        Aliquam erat volutpat. Ut quis ligula a magna blandit
        finibus.Suspendisse
      </p>
      <p class="text-center fst-italic grey">
        lacus non nunc lacinia lobortis.
      </p>
      <div class="col-12 d-flex flex-wrap">
        <CucinaryCollectionCard
          v-for="(icon, i) in icons"
          :key="i"
          :txtCCC="icon.txtI"
          :imgCCC="icon.imgI"
        />
      </div>
    </div>
  </div>
</template>

<script>
import CucinaryCollectionCard from "./CucinaryCollectionCard.vue";
export default {
  name: "cucinaryCollection",
  components: {
    CucinaryCollectionCard,
  },
  data() {
    return {
      icons: [
        {
          imgI: "drinks-recipes",
          txtI: "drinks",
        },
        {
          imgI: "soups-recipes",
          txtI: "soups",
        },
        {
          imgI: "baking-recipes",
          txtI: "bakery",
        },
        {
          imgI: "dinner-recipes",
          txtI: "dinner",
        },
        {
          imgI: "healthy-recipes",
          txtI: "healthy",
        },
        {
          imgI: "staff-picks",
          txtI: "staff picks",
        },
        {
          imgI: "premium-recipes",
          txtI: "appetisers",
        },
        {
          imgI: "quick-easy-recipes",
          txtI: "quick & easy",
        },
      ],
    };
  },
};
</script>

<style lang = "scss" scoped>
.cucinary-collection{
    margin-top:150px;
}
</style>