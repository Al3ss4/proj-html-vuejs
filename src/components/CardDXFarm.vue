<template>

      <img
        :src="require('@/assets/img/' + imgDX + '.jpg')"
        :alt="imgDX"
        class="mt-3"
      />
   
 
 
</template>

<script>
export default {
  name: "dxCardFarm",
  props: {
    imgDX: String,
  },
};
</script>

<style lang="scss" scoped>
img {
  width: 85%;
  margin-left: 65px;
}
.card-dx{
  position: relative;
  .guide{
    position: absolute;
  }
}
</style>