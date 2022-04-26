<template>
  <div class="container-fluid jumboTron">
    <div class="box-ar">
      <div class="p-5">
        <h1>Food Corner: Top Japanese Restaurants for Sushi</h1>
        <p class="date mt-4">March 25, 2019</p>
      </div>
    </div>
    <div class="pick">
      <h5 class="text-uppercase">today's pick</h5>
    </div>
  </div>
</template>

<script>
export default {
  name: "jumboTron",
};
</script>

<style lang="scss" scoped >
.jumboTron {
  background-image: url("../assets/img/single-post-img3-1200x790.jpg");
  padding: 220px;
  background-position: center;
  background-size: cover;
  position: relative;

  .pick {
    position: absolute;
    background-color: #fc7525;
    top: 28%;
    right: 44%;
    z-index: 999;
    border-radius: 10px;
    color: white;
    padding: 10px 40px;
  }
  .box-ar {
    background-color: white;
    border-radius: 10px;
    width: 700px;
    .date {
      color: #979c9c;
    }
  }
}
</style>