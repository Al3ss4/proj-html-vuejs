<template>
  <div class="container">
    <div class="row">
      <img :src="require('@/assets/img/' + imgCR + '.jpg')" :alt="imgCR" class="mt-3 w-100" />
      <div class="card">
        
        <h3 class="h4 mt-5 mx-5">{{ttlCR}}</h3>
        <span class="fst-italic mx-5">{{idCR}}</span>
        <p class="p-5">{{txtCR}}</p>
        <button type="button" class="btn btn-orange text-uppercase mx-5">learn more</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "cardRecipes",
  props: {
    imgCR: String,
    ttlCR: String,
    idCR: String,
    txtCR: String,
  },
};
</script>

<style lang="scss" scoped>
.card{
  margin-left:11px;
  max-width: 590px;
}
 .h4{
  font-size: 1.4rem;
  
}
.date{
  font-size: 0.8rem;
  
}
.btn-orange{
  background-color: orangered;
  border-radius: 0rem;
  color: white;
  max-width: 150px;
  margin-bottom: 40stpx;
}
</style>