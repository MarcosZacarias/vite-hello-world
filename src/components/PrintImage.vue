<script>
export default {
  data() {
    return {
      image: "01.webp",
    };
  },

  methods: {
    imagePath(imageName) {
      const imageURL = new URL("../assets/img/" + imageName, import.meta.url);
      return imageURL.href;
    },
  },
};
</script>

<template>
  <img :src="imagePath(image)" alt="" />
</template>

<style lang="scss" scoped>
img {
  width: 100%;
  height: 500px;

  object-fit: cover;
}
</style>
