<template>
  <div class="container mx-auto text-center">
    <div v-for="article in articles" :key="article.path">
      <a
        class="text-2xl text-primary-500 hover:text-gray-500"
        :href="`/blog${article.path}`"
        >{{ article.title }}</a
      >
      <small class="ml-4 block">Published: {{ article.date }}</small>
    </div>
  </div>
</template>

<script>
export default {
  async asyncData({ $content, params, error }) {
    const articles = await $content().fetch()
    return {
      articles,
    }
  },
  data() {
    return {
      articles: [],
    }
  },
}
</script>

<style></style>
