
<template>
  <div class="container">
    <div>
      <img
        :src="require('@/assets/img/' + imgCCSX + '.jpg')"
        :alt="imgCCSX"
        class="w-100"
      />
      <div class="h4 mt-3">{{ txtCCSX }}</div>
      <span class="date fst-italic">{{ idCCSX }} {{ monthCCSX }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "cardCollectionSX",
  props: {
    imgCCSX: String,
    txtCCSX: String,
    idCCSX: String,
    monthCCSX: String,
  },

  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.h4 {
  font-size: 1.5rem;
}
.date {
  font-size: 0.8rem;
}
</style>