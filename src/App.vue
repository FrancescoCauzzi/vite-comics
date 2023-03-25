<script setup>
import NavbarCustom from "./components/NavbarCustom.vue";
import PageContent from "./components/PageContent.vue";
import DcFeatures from "./components/DcFeatures.vue";
</script>

<template>
  <header>
    <div class="container-fluid">
      <NavbarCustom />
    </div>
  </header>

  <main>
    <div class="container-fluid __page-ctn">
      <PageContent />
    </div>
    <div class="container-fluid __features">
      <DcFeatures />
    </div>
  </main>
  <footer></footer>
</template>

<style scoped>
.__page-ctn {
  background-color: #1c1c1c;
}

.__features {
  background-color: #0282f9;
}
</style>
