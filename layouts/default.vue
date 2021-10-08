<template>
  <div class="container">
    <Nuxt />
  </div>
</template>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  line-height: 26px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background: #131313;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.container {
  margin: 0 auto;
  color: #fff;
  font-size: 1.25rem;
  max-width: 800px;
  margin: 10%;
}

h1 {
  font-size: 60px;
  line-height: 65px;
  font-weight: 400;
  letter-spacing: 1px;
  color: #fff;
  margin-bottom: 2rem;
}

img {
  width: 100%;
  height: auto;
  margin: 2rem 0;
}

p {
  margin: 1rem 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  margin: 20px 0;
}

a {
  text-decoration: none;
  color: rgb(125, 238, 204);
}

a:hover {
  text-decoration: underline;
}

.box-link {
  color: rgb(125, 238, 204);
  text-decoration: none;
  padding: 10px;
  transition: all 420ms ease-out;
}

.box-link:hover {
  background: rgb(125, 238, 204);
  color: #131313;
  transition: all 420ms ease-in;
}
</style>
