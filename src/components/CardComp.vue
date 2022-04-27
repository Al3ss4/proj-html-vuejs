<template>
  <div class="container">
 
    <div class="text-center">
    <img
      :src="require('@/assets/img/' + imgC + '.jpg')"
      :alt="imgC"
      class=" w-100 box-img"
    />

    <div class="h4 mt-3">{{ txtC }}</div>
    <span class=" date fst-italic ">{{ idC }} {{ monthC }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "cardComp",
  props: {
    imgC: String,
    txtC: String,
    idC: String,
    monthC: String,
  },

  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>

  .h4{
  font-size: 1.4rem;
  
}
.date{
  font-size: 0.8rem;
  
}



</style>