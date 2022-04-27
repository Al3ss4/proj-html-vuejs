<template>
  <div class="container">
    <div class="row">
      <div class="d-flex">
        <img
          :src="require('@/assets/img/' + imgIconDX + '.jpg')"
          :alt="imgIconDX"
          class="mt-3 ms-4"
        />
        <div class="d-flex flex-column">
          <h3 class="h4 mt-4 ms-4">{{ ttlIconDX }}</h3>
          <span class="fst-italic ms-4">{{ dateIconDX }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "iconCardDX",
  props: {
    imgIconDX: String,
    ttlIconDX: String,
    dateIconDX: String,
  },
};
</script>

<style lang="scss" scoped>
img {
  width: 75px;
  height: 75px;
  border-radius: 50%;
}
.h4 {
  font-size: 1rem;
}
.date {
  font-size: 0.5rem;
}
</style>