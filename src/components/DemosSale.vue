<template>
  <div class="container">
    <div class="row">
      <div class="d-flex flex-column square-container">
        <div class="d-flex flex-column text-center">
          <img src="../assets/img/logo.png" alt="logo" class="logo" />
          <span class="demos fw-bold">Demos</span>
        </div>
        <div class="d-flex flex-column sale">
          <span class="number text-center fw-bold">$ 39</span>
          <span class="text text-center">On Sale</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "demoSale",
};
</script>

<style lang="scss" scoped>
.square-container {
  position: absolute;
  top: 200px;
  left: 1800px;
  background-color: white;
  width: 60px;
  height: 60px;
  padding-bottom: 20px;
  border-radius: 7px;
  z-index: 9999;
 
  .logo {
    padding-top: 10px;
    padding-left: 5px;
    width: 30px;
  }
  .demos {
    font-size: 0.8rem;
    color: grey;
  }
}
 .sale {
    position: absolute;
  top: 65px;
  left: 0px;
  background-color: white;
  width: 60px;
  height: 60px;
  padding-bottom: 20px;
  border-radius: 7px;
  z-index: 9999;
     .number{
       color: green;
       font-size: 1.5rem;
     }
     .text{
       font-size: 0.8rem;
       color:grey;
     }
  }
</style>