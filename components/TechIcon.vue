<template>
  <!-- <p class="font-bold">{{ techTitle }}</p> -->
  <img class="h-10 w-10" :src="imgLocation" alt="Django Icon" />
</template>

<script>
export default {
  props: { techTitle: String, imgSrc: String },
  computed: {
    imgLocation() {
      const url = require(`@/assets/${this.imgSrc}.png`)
      return url
    },
  },
}
</script>

<style></style>
