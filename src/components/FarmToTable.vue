<template>
  <div class="container">
    <div class="row mx-4">
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
          read our blog  <span><i class="fa-solid fa-book-open-reader mx-1"></i> </span>
        </button>
      </div>
    </div>

    <CardSXFarm />
    <CardDXFarm />
  </div>
</template>

<script>
import CardSXFarm from "./CardSXFarm.vue";
import CardDXFarm from "./CardDXFarm.vue";
export default {
  name: "farmToTable",
  components: {
    CardSXFarm,
    CardDXFarm,
  },
};
</script>

<style lang="scss" scoped>
.btn-orange{
  background-color: orangered;
  border-radius: 0rem;
  color: white;
  width: 200px;
  height: 50px;
  
}
</style>