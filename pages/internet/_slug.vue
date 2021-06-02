<template>
  <article class="container">
    <h1>{{ article.title }}</h1>
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
ul {
  list-style-type: none;
  padding: 0;
}

a {
  color: rgb(125, 238, 204);
  text-decoration: none;
  padding: 10px;
  transition: all 420ms ease-out;
}
a:hover {
  background: rgb(125, 238, 204);
  color: #131313;
  transition: all 420ms ease-in;
}
li {
  margin: 20px 0;
}
</style>
