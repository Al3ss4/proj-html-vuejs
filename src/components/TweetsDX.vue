<template>
  <div class="container">
    <div class="card mt-5 p-5">
      <div class="d-flex justify-content-around">
        <h5>Tweets <a href="#"> by @Theme_Fusion</a></h5>
        <img src="@/assets/img/image.svg" alt="image" class="img-icon" />
      </div>
      <div class="row">
        <div class="col-3 d-flex mt-3">
          <img src="@/assets/img/logo.png" alt="logo" class="logo" />
          <div class="d-flex flex-column">
            <h4>ThemeFusion</h4>
            <h5 ><a href="#"><span class="grey">@Theme_Fusion</span></a></h5>
          </div>
        </div>
        <div class="col-9 d-flex justify-content-end">
          <span class="mt-3"><i class="fa-brands fa-twitter"></i></span>
        </div>
        <p class="mt-3">
          Do you need sublime WordPress hosting for vour next website? Take
          advantage of exclusive partner offers that we have secured just for
          vou. & launch your site in seconds with #avada on WP Engine hosting &
          get 30% Off this BlackFriday
          <a href="#">bit.ly/3kjLLE2 #BlackFriday2020</a>
        </p>
        <img
          src="@/assets/img/blackFriday.jpeg"
          alt="blackFriday"
          class="mt-4"
        />
        <div class="col-4 d-flex justify-content-around mt-4 mb-4">
            <img src="@/assets/img/image (2).svg" alt="heart">
            <img src="@/assets/img/image (3).svg" alt="heart">
        </div>
        <div class="col-8 d-flex justify-content-end mt-3">
            <span>21h</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "tweetComp",
};
</script>

<style lang="scss" scoped>
.logo{
    width: 30px;
    height: 30px;
}
h4{
    font-size: 1.0rem;
}
h5{
    line-height: 0px;
    a{
   text-decoration: none;
   font-size: 0.8rem;
   margin-top: 0px;
   .grey{
       color: grey;
       
   }
   }
}
.img-icon {
  width: 8%;
}
</style>