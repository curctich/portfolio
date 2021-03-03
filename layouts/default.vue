<template>
  <div>
    <Header />
    <main>
      <Nuxt />
    </main>
    <Footer />
  </div>
</template>

<script>
// export default {
// }
</script>

<style lang="scss">
/*html {*/
/*  font-family:*/
/*    'Source Sans Pro',*/
/*    -apple-system,*/
/*    BlinkMacSystemFont,*/
/*    'Segoe UI',*/
/*    Roboto,*/
/*    'Helvetica Neue',*/
/*    Arial,*/
/*    sans-serif;*/
/*  font-size: 16px;*/
/*  word-spacing: 1px;*/
/*  -ms-text-size-adjust: 100%;*/
/*  -webkit-text-size-adjust: 100%;*/
/*  -moz-osx-font-smoothing: grayscale;*/
/*  -webkit-font-smoothing: antialiased;*/
/*  box-sizing: border-box;*/
/*}*/
html {
  font-size: 62.5%;
  color: #212121;
}

a {
  text-decoration: none;
  color: #212121;
}

ul,
ol {
  margin: 0;
  padding-left: 0;
  list-style: none;
}

.inner__main {
  width: 100%;
  max-width: 748px;
  padding: 0 15px;
  margin: 0 auto;
}

.section__area {
  padding: 60px 0;
}

.title--primary {
  margin-bottom: 40px;
  font-size: 2.4rem;
  font-weight: bold;
  text-align: center;
  text-transform: uppercase;
  &::after {
    content: '';
    display: block;
    width: 32px;
    height: 4px;
    margin: 10px auto 0;
    background-color: #212121;
  }
}

.text--default {
  font-size: 1.6rem;
}
</style>
