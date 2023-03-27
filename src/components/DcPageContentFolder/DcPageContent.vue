<script>
import DcPageContentCard from "./DcPageContentCard.vue";
export default {
  data() {
    return {
      series: [],
    };
  },
  components: {
    DcPageContentCard,
  },
};
</script>
<template>
  <div class="container-fluid __page-ctn">
    <div class="container-fluid __bg-image">
      <div class="container">
        <div class="__current-series">
          <span>CURRENT SERIES</span>
        </div>
      </div>
    </div>
    <div class="container py-5 text-start">
      <DcPageContentCard />
      TESTO PROVA
    </div>
  </div>
</template>
<style scoped>
.__page-ctn {
  /* text-align: start; */
  color: white;
  font-size: 1.3em;
  font-weight: bold;
  padding-left: 0;
  padding-right: 0;

  background-color: #1c1c1c;
}

.__bg-image {
  background-image: url(/img/jumbotron.jpg);
  height: 400px;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}
.__current-series {
  position: absolute;
  bottom: -5%;

  padding: 5px 15px 5px 15px;
  background-color: #0282f9;
}
</style>
