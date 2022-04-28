
<template>
  <div class="container">
    <div class="card-cont">
      <img
        :src="require('@/assets/img/' + imgCCSX + '.jpg')"
        :alt="imgCCSX"
        class="w-100"
      />
      <div class="hover-img fw-bold">
        <div class="d-flex flex-column">
          <span class="link"><i class="fas fa-link mt-3"></i></span>
         <span class="text-center"> {{ txtCCSX }}</span>
        </div>
        </div>
        <div class="h4 mt-3">{{ txtCCSX }}</div>
        <span class="date fst-italic">{{ idCCSX }} {{ monthCCSX }}</span>
      </div>
    </div>
  <!--</div>-->
</template>

<script>
export default {
  name: "cardCollectionSX",
  props: {
    imgCCSX: String,
    txtCCSX: String,
    idCCSX: String,
    monthCCSX: String,
  },

  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.card-cont {
  position: relative;

  .hover-img {
    display: none;
    position: absolute;
    top: 0;
    padding: 80px;
    background-color: #fc7525;
    width: 100%;
    opacity: 0.8;
    height: 251px;
    cursor: pointer;
    .link{
      width: 50px;
      height: 50px;
      border-radius:50%;
      background-color: white;
      color: #fc7525;
      margin-left: 80px;
      margin-bottom:15px;
      padding-left: 15px ;
    }
  }
}

.card-cont:hover .hover-img {
  display: block;
  font-size: 1rem;
  color: white;
}
.h4 {
  font-size: 1.8rem;
}
.date {
  font-size: 0.8rem;
}
</style>