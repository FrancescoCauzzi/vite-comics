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
  <div class="__nav-bar-cnt d-flex align-items-center">
    <div class="__logo-wrapper w-25 p-3">
      <img src="/img/dc-logo.png" alt="cannot-render-image" srcset="" />
    </div>
    <div class="__links-wrapper w-75">
      <ul class="d-flex gap-4">
        <li
          class="fw-bold d-flex align-items-center"
          v-for="link in linksList"
          :key="link.id"
        >
          <a href="">
            {{ link.toUpperCase() }}
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.__nav-bar-cnt {
  height: 135px;
}
a {
  cursor: pointer;
  text-decoration: none;
  color: black;
}

.__links-wrapper {
  height: 100%;
}

ul {
  height: 100%;
}
li {
  height: 100%;
}

li:hover {
  border-bottom: 5px solid #0282f9;
  padding-top: 5px;
  color: #0282f9;
}
</style>
