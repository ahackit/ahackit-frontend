<template>
  <div class="flex flex-col items-center h-10 w-10">
    <!-- <p class="font-bold">{{ techTitle }}</p> -->
    <img :src="imgLocation" alt="Django Icon" />
  </div>
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
