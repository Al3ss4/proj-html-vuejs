<template>
  <header class="container">
    <div class="row">
      <div class="menu-sx col-10 d-flex justify-content-start">
        <li v-for="(element, i) in menuSx" :key="i" class="m-3">
          <a href="#">{{ element }}</a>
        </li>
      </div>

      <div class="col-2 d-flex justify-content-between align-items-center social">
        <span><i class="fa-brands fa-facebook"></i></span>
        <span><i class="fa-brands fa-instagram"></i></span>
        <span><i class="fa-brands fa-twitter"></i></span>
        <span><i class="fa-brands fa-youtube"></i></span>
      </div>
    </div>

    <div class="d-flex justify-content-center p-3">
      <div class="p-2">
        <img src="../assets/img/avada-food-logo.png" alt="Logo" />
      </div>
    </div>
    <div>
      <ul class="d-flex fw-bold justify-content-between col-12 mt-3">
        <li class="m-3 grid" v-for="(element, i) in menu" :key="i" :class="{'grid': element.menu === 'Home'}">
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
      menuSx: ["Dowload App ", "Advertise with us"],
    };
  },
  methods:{
    style(i){
      switch(i) {
        case 'Home':
          return{
            backgroundColor:'grid'
          }
      }
    }
  }
};
</script>

<style lang="scss" scoped>
.menu-sx {
    a{
  color: #afafaf;
 
  }
 
}
  .social{
    color: #afafaf;
  }
li {
  font-size: 14px;

}
.grid{
  color:red
}


</style> 