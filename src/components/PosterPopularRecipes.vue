<template>
  <img
    :src="require('@/assets/img/' + imgPR + '.jpg')"
    :alt="imgPR"
    class=" p-3"
  />
</template>

<script>
export default {
  name: "posterRecipes",
  props: {
    imgPR: String,
  },
};
</script>

<style lang="scss" scoped>
img{
  width: 48%;
}
</style>