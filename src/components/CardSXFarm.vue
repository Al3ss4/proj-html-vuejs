<template>
  <div class="container">
    <div class="row">
      <div class="card-cont">
      <img
        :src="require('@/assets/img/' + imgSX + '.jpg')"
        :alt="imgSX"
        class="mt-3 w-100"
      />
      <div class="hover-img fw-bold">
        <div class="d-flex flex-column">
          <span class="link"><i class="fas fa-link mt-3"></i></span>
          {{ txtSX }}
        </div>
      </div>
   </div>
        <h3 class="h4 mt-5 mx-5">{{ ttlSX }}</h3>
        <span class="fst-italic mx-5">{{ idSX }} {{dateSX}}</span>
        <p class="p-5">{{ txtSX }}</p>
        <div class="mx-5 mb-4 d-flex justify-content-between">
          <p>Read More ></p>
          <span><i class="fa-brands fa-rocketchat"></i></span>
        </div>
      
    </div>
  </div>
</template>

<script>
export default {
  name: "iconCardSX",
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
    top: 15px;
    
    padding: 150px;
    background-color: #fc7525;
    width: 808px;
    opacity: 0.8;
    height: 533px;
    cursor: pointer;
    .link{
      width: 50px;
      height: 50px;
      border-radius:50%;
      background-color: white;
      color: #fc7525;
      margin-left: 225px;
      margin-bottom:15px;
      padding-left: 12px;
    }
  }
}

.card-cont:hover .hover-img {
  display: block;
  font-size: 1.2rem;
  color: white;
}
</style>