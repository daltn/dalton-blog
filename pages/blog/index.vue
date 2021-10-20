<template>
  <section class="container">
    <h1>blog :)</h1>
    <ul>
      <li v-for="article of articles" :key="article.slug">
        <NuxtLink :to="{ name: 'blog-slug', params: { slug: article.slug } }">
          <h3>{{ article.title }}</h3>
        </NuxtLink>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const articles = await $content('blog')
      .only(['title', 'description', 'img', 'slug', 'author'])
      .sortBy('createdAt', 'desc')
      .fetch()

    return {
      articles,
    }
  },
}
</script>
<style scoped>
h3 {
  font-weight: 500;
}
</style>
