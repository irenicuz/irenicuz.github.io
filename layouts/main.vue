<template>
  <div class="body">
    <Header />
    <main class="content">
      <nuxt />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from '~/components/Header'
import Footer from '~/components/Footer'
export default {
  components: {
    Header, Footer
  }
}

</script>

<style lang="scss">

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

html {
  font-family: 'Roboto', sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  color: #333;

  //background-color: #252934;
}

main {
    display: flex;
    max-width: 900px;
    margin-left: auto;
    margin-right: auto;
    padding: 30px 10px;
}

h1, h2 {
  font-family: 'Rubik', sans-serif;
}

h1 {
  font-size: 48px;
  margin-bottom: 20px;
}

p {
  font-size: 22px;
  margin-bottom: 15px;
  font-family: 'Source Sans Pro', sans-serif;
  max-width: 700px;
}

a {
  text-decoration: none;
  color: #333;
}

img {
  max-width: 300px;

  @media screen and (max-width: 700px){
    max-width: 100%;
  }
}

</style>
