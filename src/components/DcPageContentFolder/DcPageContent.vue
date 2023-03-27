<script>
import DcPageContentCard from "./DcPageContentCard.vue";
import data from "../../../public/dc-comics.json";
console.log(data);
export default {
  data() {
    return {
      cards: data,
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
          <span>CURRENT SERIES ER</span>
        </div>
      </div>
    </div>
    <div class="container py-5">
      <DcPageContentCard></DcPageContentCard>
    </div>
    <div class="__btn-container text-center">
      <button id="load-more-btn">LOAD MORE</button>
    </div>
  </div>
</template>
<style scoped>
.__page-ctn {
  /* text-align: start; */
  color: white;
  font-size: 1.3em;
  font-weight: bold;
  padding: 0px 0px 20px 0px;

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

  padding: 5px 20px 5px 20px;
  background-color: #0282f9;
}

#load-more-btn {
  padding: 5px 40px 5px 40px;
  background-color: #0282f9;
  font-weight: bold;
}
</style>
