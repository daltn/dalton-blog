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
  word-spacing: 1px;
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
  font-size: 4rem;
  font-weight: 400;
  letter-spacing: 1px;
  color: #fff;
  margin-bottom: 2rem;
}

p {
  margin: 1rem 0;
}
</style>
