<template>
  <div class="container test-ar mt-5 mb-5">
    <div class="row">
      <div class="d-flex justify-content-center">
        <b-carousel
          id="carousel-1"
          v-model="slide"
          :interval="3000"
          controls
          indicators
          background="#f0eeeb"
          style="text-shadow: 1px 1px 2px #f0eeeb"
          @sliding-start="onSlideStart"
          @sliding-end="onSlideEnd"
        >
          <b-carousel-slide>
            <template v-slot:img>
              <img
                class="d-block img-fluid ciao"
              
                src="@/assets/img/Yogurt-Nan-200x132.jpg"
                alt="image slot"
              />
            </template>
          </b-carousel-slide>
          <b-carousel-slide>
            <template v-slot:img>
              <img
                class="d-block img-fluid ciao"
                
                src="@/assets/img/Mixed-fruits-200x132.jpg"
                alt="image slot"
              />
            </template>
          </b-carousel-slide>
          <b-carousel-slide>
            <template v-slot:img>
              <img
                class="d-block img-fluid ciao"
                src="@/assets/img/r-rachel-park-366508-unsplash-min-200x132.jpg"
                alt="image slot"
              />
            </template>
          </b-carousel-slide>
          <b-carousel-slide>
            <template v-slot:img>
              <img
                class="d-block img-fluid ciao"
                src="@/assets/img/r-michelle-tsang-500721-unsplash-min-200x132.jpg"
                alt="image slot"
              />
            </template>
          </b-carousel-slide>
        </b-carousel>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "carouselComp",
  data() {
    return {
      slide: 0,
      sliding: null,
    };
  },
  methods: {
    onSlideStart() {
      this.sliding = true;
    },
    onSlideEnd() {
      this.sliding = false;
    },
  },
};
</script>

<style lang="scss" scoped>
.test-ar{
    height: 600px;
}
.ciao {
  width: 500px;
}
</style>