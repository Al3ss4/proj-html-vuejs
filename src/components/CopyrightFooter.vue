<template>
  <div class="container-fluid">
    <div class="row">
      <div class="d-flex col-1 justify-content-start">
        <span class="arrow"> <a href="#"><i class="fas fa-chevron-circle-up"></i></a></span>
      </div>
      <div class="d-flex col-10 justify-content-center align-items-center">
        <p>
          © Copyright 2012 - 2020 | Avada Theme by ThemeFusion/ All Rights
          Reserved | Powered by WordPress
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "copyFooter",
};
</script>

<style lang="scss" scoped>
.container-fluid {
  color: grey;
  a{
      color: grey;
  }
  .arrow {
    font-size: 70px;
  }
}
</style>