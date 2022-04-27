<template>
  <div class="container">
    <div class="row">
      <img
        :src="require('@/assets/img/' + imgSX + '.jpg')"
        :alt="imgSX"
        class="mt-3 w-100"
      />
      <div class="card">
        <h3 class="h4 mt-5 mx-5">{{ ttlSX }}</h3>
        <span class="fst-italic mx-5">{{ idSX }} {{dateSX}}</span>
        <p class="p-5">{{ txtSX }}</p>
        <div class="mx-5 mb-4 d-flex justify-content-between">
          <p>Read More ></p>
          <span><i class="fa-brands fa-rocketchat"></i></span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "sxCardFarm",
  props: {
    imgSX: String,
    ttlSX: String,
    idSX: String,
    txtSX: String,
    dateSX: String,
  },
};
</script>

<style lang="scss" scoped>
.card {
  margin-left: 11px;
  max-width: 810px;
}
.h4 {
  font-size: 1.4rem;
}
.date {
  font-size: 0.8rem;
}
.btn-orange {
  background-color: orangered;
  border-radius: 0rem;
  color: white;
  max-width: 150px;
  margin-bottom: 40px;
}
</style>