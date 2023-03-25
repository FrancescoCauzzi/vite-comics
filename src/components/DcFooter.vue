<script>
export default {
  data() {
    return {
      footerItems: [
        {
          title: "dc comics",
          links: [
            "Characters",
            "Comics",
            "Movies",
            "TV",
            "Games",
            "Videos",
            "News",
          ],
        },

        {
          title: "dc",
          links: [
            "Terms of Use",
            "Privacy Policy (Nes)",
            "Ad Choices",
            "Advertising",
            "Jobs",
            "Subcriptions",
            "Talent Workshops",
            "CPSC Certificates",
            "Ratings",
            "Shop Help",
            "Contact Us",
          ],
        },
        {
          title: "sites",
          links: [
            "DC",
            "MAD Magazine",
            "DC Kids",
            "DC Universe",
            "DC Power Visa",
          ],
        },
        {
          title: "shop",
          links: ["Shop DC", "Shop DC Collectibles"],
        },
      ],
    };
  },
};
</script>
<template>
  <div class="container __footer-cnt">
    <div class="row row-cols-3 py-3 w-50">
      <div
        v-for="(item, index) in footerItems"
        :key="index"
        class="col __links"
      >
        <ul :class="`__${item.title.replace(/\s+/g, '')}`">
          <h5 class="text-white mb-2">{{ item.title.toUpperCase() }}</h5>
          <li
            class="__link text-white py-1"
            v-for="(link, index) in item.links"
            :key="index"
          >
            <a href="">{{ link }}</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<style scoped>
a {
  text-decoration: none;
  cursor: pointer;
  color: #898989;
}

.__link {
  margin-bottom: -8px;
}

.__shop {
  margin-top: -80px;
}
</style>
