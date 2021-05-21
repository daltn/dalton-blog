<template>
  <article class="blog-container">
    <nuxt-content :document="article" />
  </article>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const article = await $content('internet', params.slug).fetch()

    return { article }
  },
}
</script>

<style>
.container {
  margin: 20%;
  color: #fff;
  font-size: 1.5rem;
}
</style>
