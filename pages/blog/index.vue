<template>
  <div class="container mx-auto text-center">
    <a
      v-for="article in articles"
      :key="article.path"
      :href="`/blog${article.path}`"
      >{{ article.title }}</a
    >
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
