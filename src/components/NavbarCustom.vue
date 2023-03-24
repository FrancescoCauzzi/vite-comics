<script>
export default {
  data() {
    return {
      linksList: [
        "characters",
        "comics",
        "movies",
        "tv",
        "games",
        "collectibles",
        "videos",
        "fans",
        "news",
        "shop",
      ],
    };
  },
};
</script>

<template>
  <div class="__nav-bar-cnt d-flex p-3 align-items-center">
    <div class="__logo-wrapper w-25">
      <img src="/img/dc-logo.png" alt="cannot-render-image" srcset="" />
    </div>
    <div class="__links-wrapper w-75">
      <ul class="d-flex gap-4 flex-wrap">
        <li class="fw-bold" v-for="link in linksList" :key="link.id">
          <a href="">
            {{ link.toUpperCase() }}
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
a {
  cursor: pointer;
  text-decoration: none;
  color: black;
}
</style>
