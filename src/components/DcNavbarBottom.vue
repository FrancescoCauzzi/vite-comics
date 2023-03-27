<script>
export default {
  data() {
    return {
      btnText: "sign-up now",
      socialMediaLinksTitle: "follow us",
      socialMediaLinks: [
        { title: "facebook", url: "", image: "/img/footer-facebook.png" },
        { title: "twitter", url: "", image: "/img/footer-twitter.png" },
        { title: "youtube", url: "", image: "/img/footer-youtube.png" },

        { title: "pinterest", url: "", image: "/img/footer-pinterest.png" },
        { title: "periscope", url: "", image: "/img/footer-periscope.png" },
      ],
    };
  },
};
</script>
<template>
  <div class="container d-flex justify-content-between">
    <div class="__left d-flex py-3">
      <button class="p-2">{{ btnText.toUpperCase() }}</button>
    </div>
    <div class="__right d-flex justify-content-end p-3">
      <div class="__social-media d-flex align-items-center">
        <h5 class="__social-media-title">
          {{ socialMediaLinksTitle.toUpperCase() }}
        </h5>
        <ul class="d-flex gap-3">
          <li class="" v-for="(item, index) in socialMediaLinks" :key="index">
            <img class="" :src="item.image" alt="" />
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<style scoped>
button {
  background-color: transparent;
  border: 2px solid #0282f9;
}
.__social-media-title {
  color: #0282f9;
}

li {
  cursor: pointer;
}

img {
  padding-top: 12px;
}
</style>
