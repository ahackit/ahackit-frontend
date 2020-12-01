<template>
  <div class="container mx-auto text-center">
    <nuxt-content :document="page" />
  </div>
</template>

<script>
export default {
  async asyncData({ $content, params, error }) {
    const slug = params.slug || 'index'
    const page = await $content(slug).fetch()
    return {
      page,
    }
  },
  data() {
    return {
      page: {},
    }
  },
}
</script>

<style></style>
