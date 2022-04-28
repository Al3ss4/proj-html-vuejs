<template>
  <div class="container">
    <div class="row">
      <div class="card-cont">
        <img
          :src="require('@/assets/img/' + imgCR + '.jpg')"
          :alt="imgCR"
          class="mt-3 w-100"
        />
        <div class="hover-img fw-bold">
          <div class="d-flex flex-column">
            <span class="link"><i class="fas fa-link mt-3"></i></span>
            {{ ttlCR }}
          </div>
        </div>
      </div>
      <div class="card">
        <h3 class="h4 mt-5 mx-5">{{ ttlCR }}</h3>
        <span class="fst-italic mx-5">{{ idCR }}</span>
        <p class="p-5">{{ txtCR }}</p>
        <button type="button" class="btn btn-orange text-uppercase mx-5">
          learn more
        </button>
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
.card {
  margin-left: 11px;
  max-width: 590px;
}
.h4 {
  font-size: 1.4rem;
}
.date {
  font-size: 0.8rem;
}
.btn-orange {
  background-color: #fc7525;
  border-radius: 0rem;
  color: white;
  max-width: 150px;
  margin-bottom: 40px;
}
.card-cont {
  position: relative;
  .hover-img {
    display: none;
    position: absolute;
    top: 16px;
    right: 12px;
    padding: 160px;
    background-color: #fc7525;
    width: 96%;
    opacity: 0.8;
    height: 100%;
    .link {
      width: 80px;
      height: 80px;
      border-radius: 50%;
      background-color: white;
      color: #fc7525;
      margin-left: 100px;
      padding-left: 25px;
      padding-top: 12px;
      margin-bottom: 15px;
    }
  }
}

.card-cont:hover .hover-img {
  display: block;
  font-size: 1.5rem;
  color: white;
}
</style>