<template>
  <div class="container">
      <div class="row">
            
             <img
        :src="require('@/assets/img/' + imgFtr + '.png')"
        :alt="imgFtr"
        class="mt-3"
      />
      </div>
  </div>
</template>

<script>
export default {
name:"appFooter",
props:{
    imgFtr:String
}
}
</script>

<style>

</style>