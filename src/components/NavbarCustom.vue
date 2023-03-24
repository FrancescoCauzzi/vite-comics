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

<template lang="html">
  <div class="__nav-bar-cnt d-flex">
    <div class="__logo-wrapper w-50">
      <img src="/img/dc-logo.png" alt="cannot-render-image" srcset="" />
    </div>
    <div class="__links-wrapper w-50">
      <ul class="d-flex gap-4">
        <li v-for="link in linksList" :key="link.id">
          {{ link }}
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped></style>
