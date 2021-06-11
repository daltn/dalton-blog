<template>
  <article class="container">
    <h1>{{ article.title }}</h1>
    <p class="date">{{ formatDate(article.updatedAt) }}</p>
    <nuxt-content :document="article" />
  </article>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const article = await $content('blog', params.slug).fetch()

    return { article }
  },
  methods: {
    formatDate(date) {
      const options = { year: 'numeric', month: 'long', day: 'numeric' }
      return new Date(date).toLocaleDateString('en', options)
    },
  },
}
</script>

<style>
.date {
  padding-bottom: 5px;
  border-bottom: 1px solid rgb(125, 238, 204);
}
</style>
