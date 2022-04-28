<template>
  <div class="container">
    <div class="text-center card-cont">
      <img
        :src="require('@/assets/img/' + imgC + '.jpg')"
        :alt="imgC"
        class="w-100"
      />
      <div class="hover-img fw-bold">
        <div class="d-flex flex-column">
          <span class="link"><i class="fas fa-link mt-3"></i></span>
          {{ txtC }}
        </div>
      </div>

      <div class="h4 mt-3">{{ txtC }}</div>
      <span class="date fst-italic">{{ idC }} {{ monthC }}</span>
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
    height: 71%;
    .link{
      width: 50px;
      height: 50px;
      border-radius:50%;
      background-color: white;
      color: #fc7525;
      margin-left: 80px;
      margin-bottom:15px;
    }
  }
}

.card-cont:hover .hover-img {
  display: block;
  font-size: 1rem;
  color: white;
}
.h4 {
  font-size: 1.4rem;
}
.date {
  font-size: 0.8rem;
}
</style>