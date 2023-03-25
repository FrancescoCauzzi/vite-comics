<script>
export default {
  data() {
    return {
      message: "<-- Content goes here -->",
    };
  },
};
</script>
<template>
  <div class="container __page-ctn">
    <p>{{ message }}</p>
  </div>
</template>
<style scoped>
.__page-ctn {
  padding: 40px 0 40px 0;
  text-align: start;
  color: white;
  font-size: 1.3em;
  font-weight: bold;
}
</style>
