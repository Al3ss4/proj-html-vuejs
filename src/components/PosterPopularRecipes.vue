<template>
<div class="card-cont">
  <img
    :src="require('@/assets/img/' + imgPR + '.jpg')"
    :alt="imgPR"
    class=" p-3 w-100"
  />

<div class="hover-img fw-bold">
        <div class="d-flex flex-column">
          <span class="link"><i class="fas fa-link mt-3"></i></span>
          {{ txtPR }}
        </div>
      </div>
</div>

</template>

<script>
export default {
  name: "posterRecipes",
  props: {
    imgPR: String,
    txtPR: String
  },
};
</script>

<style lang="scss" scoped>
.card-cont {
  position: relative;

  .hover-img {
    display: none;
    position: absolute;
    top: 16px;
    right: 15px;
    padding: 35px;
    background-color: #fc7525;
    width: 90%;
    opacity: 0.8;
    height: 86%;
    cursor: pointer;
    .link{
      width: 50px;
      height: 50px;
      border-radius:50%;
      background-color: white;
      color: #fc7525;
      margin-left: 80px;
      margin-bottom:15px;
      padding-left: 13px;
    }
  }
}

.card-cont:hover .hover-img {
  display: block;
  font-size: 1rem;
  color: white;
}
img{
  width: 48%;
}
</style>