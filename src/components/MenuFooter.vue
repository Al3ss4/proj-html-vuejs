<template>
  <div class="container">
    <div class="row">
      <ul class="d-flex mt-4 fw-bold flex-column ">
        <li v-for="(element, i) in menu" :key="i" class="mt-3 mx-5">
          <a href="#">{{ element }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "menuFooter",
  data() {
    return {
      menu: ["Home", "Recipes", "Places", "Blog", "About", "Contact"],
    };
  },
};
</script>

<style>
</style>