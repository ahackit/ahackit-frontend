<template>
  <div class="flex flex-col rounded-lg shadow-lg overflow-hidden m-4 md:w-1/3">
    <a :href="'google.com'">
      <div class="flex-shrink-0">
        <img class="h-48 w-full object-cover" :src="imgLocation" alt />
      </div>
      <div class="flex-1 bg-white p-6 flex flex-col justify-between">
        <div class="flex-1">
          <a href="#" class="block">
            <h3 class="mt-2 text-xl leading-7 font-semibold text-primary-500">
              {{ title }}
            </h3>
            <p class="mt-3 text-base leading-6 text-gray-500">
              <slot></slot>
            </p>
          </a>
        </div>
        <h1 class="mt-6 text-primary-500">Technologies</h1>
        <div class="flex justify-center">
          <TechIcon tech-title="Vue" img-src="vueicon"></TechIcon>
        </div>
      </div>
    </a>
  </div>
</template>

<script>
import TechIcon from '@/components/TechIcon'
export default {
  name: 'Card',
  components: [TechIcon],
  props: {
    image: {
      type: String,
    },
    title: {
      type: String,
    },
    link: {
      type: String,
    },
  },
  computed: {
    imgLocation() {
      const url = require(`@/assets/${this.image}.png`)
      return url
    },
  },
}
</script>

<style></style>
