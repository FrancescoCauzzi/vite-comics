<script>
export default {
  data() {
    return {
      features: [
        {
          name: "digital comics",
          imageSrc: "/img/buy-comics-digital-comics.png",
        },
        {
          name: "dc merchandise",
          imageSrc: "/img/buy-comics-merchandise.png",
        },
        {
          name: "subscription",
          imageSrc: "/img/buy-comics-subscriptions.png",
        },
        {
          name: "comic shop locator",
          imageSrc: "/img/buy-comics-shop-locator.png",
        },
        {
          name: "dc power visa",
          imageSrc: "/img/buy-dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>
<template>
  <div class="container py-5">
    <div class="row row-cols-5 __features-ctn text-white">
      <div
        v-for="(item, index) in features"
        :key="index"
        class="col d-flex align-items-center __col"
      >
        <img class="" :src="item.imageSrc" alt="cannot retrieve image" />
        <div class="__name px-2">{{ item.name.toUpperCase() }}</div>
      </div>
    </div>
  </div>
</template>
<style scoped>
img {
  object-fit: contain;
  height: 3.5em;
  /* width: 50%; */
}

.__name {
  font-size: 0.8em;
}
.__col {
  cursor: pointer;
}
</style>
