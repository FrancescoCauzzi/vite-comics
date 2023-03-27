<script>
// Object API, be careful not to confuse this syntax with the one of the 'Composition API'
import DcNavbarCustom from "./components/DcNavbarCustom.vue";
import DcPageContent from "./components/DcPageContent.vue";
import DcFeatures from "./components/DcFeatures.vue";
import DcFooter from "./components/DcFooter.vue";
import DcNavbarBottom from "./components/DcNavbarBottom.vue";
export default {
  data() {
    return {};
  },
  components: {
    DcNavbarCustom,
    DcPageContent,
    DcFeatures,
    DcFooter,
    DcNavbarBottom,
  },
};
</script>

<template>
  <header>
    <div class="container-fluid">
      <DcNavbarCustom />
    </div>
  </header>

  <main>
    <div class="container-fluid __page-ctn">
      <DcPageContent />
    </div>
    <div class="container-fluid __features">
      <DcFeatures />
    </div>
  </main>
  <footer>
    <div class="container-fluid __footer position-relative">
      <DcFooter />
    </div>
    <div class="container-fluid __navbar-bottom">
      <DcNavbarBottom />
    </div>
  </footer>
</template>

<style scoped>
.__footer {
  background-image: url(/img/footer-bg.jpg);

  overflow: hidden;
}
.__page-ctn {
  background-color: #1c1c1c;
}

.__features {
  background-color: #0282f9;
}

.__navbar-bottom {
  background-color: #303030;
}
</style>
