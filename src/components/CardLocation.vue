<template>
     <div class="card-dx">
      <img
        :src="require('@/assets/img/' + imgLocation + '.jpg')"
        :alt="imgLocation"
        class="mt-3"
      />
      <span class="guide"> City Guide: Singapore</span>
      <button type="button" class="btn btn-orange text-uppercase"><i class="fas fa-globe-asia mx-1"></i>view all city guides</button>
    </div>
</template>

<script>
export default {
name:"singaporeCard",
props:{
    imgLocation:String
}
}
</script>

<style lang="scss" scoped>
img {
  width: 85%;
  margin-left: 65px;
}
.card-dx{
  position: relative;
  margin-top: 20px;
  .guide{
    position: absolute;
    top: 150px;
    left: 65px;
    background-color: black;
    color: white;
    font-size: 1.4rem;
    padding: 10px;
    opacity: 0.8;
  }
  .btn-orange {
  background-color: #fc7525;;
  border-radius: 0rem;
  color: white;
  width: 85%;
  height: 50px;
  margin-left: 65px;
}
}
</style>