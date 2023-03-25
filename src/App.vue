<script setup>
import DcNavbarCustom from "./components/DcNavbarCustom.vue";
import DcPageContent from "./components/DcPageContent.vue";
import DcFeatures from "./components/DcFeatures.vue";
import DcFooter from "./components/DcFooter.vue";
import DcNavbarBottom from "./components/DcNavbarBottom.vue";
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
      <img
        id="dc-logo-bg"
        src="/img/dc-logo-bg.png"
        alt="Cannot retrieve image"
      />
    </div>
    <div class="container-fluid __navbar-bottom">
      <DcNavbarBottom />
    </div>
  </footer>
</template>

<style scoped>
.__page-ctn {
  background-color: #1c1c1c;
}

.__features {
  background-color: #0282f9;
}

.__footer {
  background-image: url(/img/footer-bg.jpg);

  overflow: hidden;
}

#dc-logo-bg {
  position: absolute;
  right: 10%;
  bottom: -25%;
  z-index: 0;
}

.__navbar-bottom {
  background-color: #303030;
}
</style>
