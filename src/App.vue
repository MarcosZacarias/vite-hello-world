<script>
import PrintImage from "./components/PrintImage.vue";

export default {
  data() {
    return {
      message: "Hello Word",
    };
  },

  components: { PrintImage },
};
</script>

<template>
  <h1>{{ message }}</h1>
  <PrintImage></PrintImage>
</template>

<style lang="scss" scoped>
h1 {
  color: rgb(102, 38, 38);
}
</style>
