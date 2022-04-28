<template>
  <div class="container mt-3">
    <div class="row">
      <div class="col-5 m-ar">
        <h4 class="orange">Follow Us</h4>
        <div class="d-flex justify-content-between social mt-4 px-1">
          <span><i class="fa-brands fa-facebook"></i></span>
          <span><i class="fa-brands fa-instagram"></i></span>
          <span><i class="fa-brands fa-twitter"></i></span>
          <span><i class="fa-brands fa-youtube"></i></span>
          <span><i class="fab fa-pinterest-p"></i></span>
        </div>
      </div>
    </div>
    <div class="m-ar mt-4">
      <button type="button" class="btn btn-social bg-white btn-lg">
        Popular
      </button>
      <button type="button" class="btn btn-social bg-grey btn-lg">
        Recent
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "socialComp",
};
</script>

<style lang="scss" scoped>
.m-ar {
  margin-left: 39px;
}
.social {
  color: #afafaf;
}
.btn-social {
  width: 164px;
  border: 1px solid #f0eeeb;
  border-radius: 0rem;
  .bg-white {
    background-color: white;
  }
}
</style>