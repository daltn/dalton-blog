<template>
  <section class="container">
    <h1>dalton saffe</h1>
    <div class="links">
      <!-- <nuxt-link to="/blog">blog</nuxt-link> -->
      <nuxt-link to="/internet">internet</nuxt-link>
      <a href="mailto:daltonsaffe@gmail.com">contact</a>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style>
.links {
  display: flex;
  justify-content: space-between;
  margin-top: 50px;
  max-width: 400px;
}
.links a {
  color: rgb(125, 238, 204);
  text-decoration: none;
  padding: 10px;
  transition: all 420ms ease-out;
}
.links a:hover {
  background: rgb(125, 238, 204);
  color: #131313;
  transition: all 420ms ease-in;
}
</style>
