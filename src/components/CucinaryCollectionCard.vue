<template>
  <div class="d-flex flex-column card-ar">
    <img
      :src="require('@/assets/img/' + imgCCC + '.png')"
      :alt="imgCCC"
      class="p-3"
    />
  

    <span class="text-center text-uppercase">{{ txtCCC }}</span>
      <div class="hover-img fw-bold text-center text-uppercase">{{ txtCCC }}</div>
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
.card-ar {
  background-color: white;
  margin: 20px;
  padding: 20px 45px;
  position: relative;
}
.hover-img {
  display: none;
  position: absolute;
  top: 200px;
  right: 70px;
  background-color: #fc7525;
  width: 50%;
  height: 20%;
}
.card-ar:hover .hover-img {
  display: block;
  font-size: 1rem;
  color: white;
  padding-top:10px;
}
</style>