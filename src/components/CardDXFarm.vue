<template>
<img
    :src="require('@/assets/img/' + imgDX + '.jpg')"
    :alt="imgDX"
    class=" mt-3 w-100"
  />
</template>

<script>
export default {
name:"dxCardFarm",
props:{
  imgDX: String,
}
}
</script>

<style lang="scss" scoped>

</style>