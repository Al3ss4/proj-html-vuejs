<template>
  <footer>
    <div class="container mb-5">
      <div class="row">
        <div class="col-3">
          <SocialFooter />
        </div>
        <div class="col-3">
          <MenuFooter />
        </div>
        <div class="col-3">
          <ContactFooter />
        </div>
        <div class="col-3">
          <h5 class="text-uppercase orange mt-5 mx-4">get our app!</h5>
          <AppFooter
            v-for="(element, i) in elements"
            :key="i"
            :imgFtr="element.imgFot"
          />
        </div>
      </div>
    </div>
    <div class="container-fluid">
      <CopyrightFooter />
    </div>
  </footer>
</template>

<script>
import SocialFooter from "./SocialFooter.vue";
import MenuFooter from "./MenuFooter.vue";
import ContactFooter from "./ContactFooter.vue";
import AppFooter from "./AppFooter.vue";
import CopyrightFooter from "./CopyrightFooter.vue";
export default {
  name: "footerComp",
  components: {
    SocialFooter,
    MenuFooter,
    ContactFooter,
    AppFooter,
    CopyrightFooter,
  },
  data() {
    return {
      elements: [
        {
          imgFot: "download-android-200x66",
        },
        {
          imgFot: "download-app-store-200x66",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
</style>