<template>
  <header>
  
    <div class="d-flex justify-content-center p-3">
      <div class="p-2">
        <img src= "../assets/img/avada-food-logo.png" alt="Logo" />
      </div>
    </div>
    <div>
      <ul class="d-flex text-uppercase fw-bold justify-content-center">
        <li v-for="(element, i) in menu" :key="i" class="m-3">
          <a href="#">{{ element }}</a>
        </li>
         <span class="my-3"><i class="fa-solid fa-magnifying-glass"></i></span>
      
      </ul>
    </div>
  </header>
</template>


<script>
export default {
  name: "HeaderComp",
  data() {
    return {
      menu: ["Home", "Recipes", "Places", "Blog", "About", "Contact"],
    };
  },
};
</script>

<style lang="scss">
li {
  font-size: 14px;
}
</style> 