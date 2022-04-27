<template>
  <div class="d-flex flex-column card-ar">
    <img
      :src="require('@/assets/img/' + imgCCC + '.png')"
      :alt="imgCCC"
      class="p-3"
    />
    <span class="text-center text-uppercase">{{ txtCCC }}</span>
  </div>
</template>

<script>
export default {
  name: "collectionCard",
  props: {
    imgCCC: String,
    txtCCC: String,
  },
};
</script>

<style lang="scss" scoped>
.card-ar{
    background-color: white;
    margin:20px;
   padding: 20px 45px;
  
    
}
</style>