<script>
export default {
  data() {
    return {
      name: "DCPageContentCard",
    };
  },
  props: {
    image: String,
    genre: String,
  },
};
</script>
<template>
  <div class="__card">
    <div class="__img-card-container">
      <img :src="image" alt="Cannot Retrieve Image" />
    </div>
    <!-- le prop vengono interpolate e chiamate come delle semplici proprietà in data() -->
    <div class="__genre">{{ genre.toUpperCase() }}</div>
  </div>
</template>
<style scoped>
.__card {
  width: calc(100% / 6 * 1 - (10px / 6 * 5));

  min-width: 130px;
}

img {
  width: 100%;
  aspect-ratio: 1 / 1;
  /* height: 100%; */
  object-fit: cover;
  object-position: top;
}
.__img-card-container {
  /* background-color: red; */
  /* height: 180px; */
  overflow: hidden;

  margin-bottom: 10px;
}
</style>
