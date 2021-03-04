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
export default {
  mounted() {
    this.$nextTick(function () {
      this.$adobeFonts(document)
    })
  },
}
</script>

<style lang="scss">
html {
  font-size: 62.5%;
  visibility: hidden;
}

html.wf-active {
  visibility: visible;
}

body {
  font-family: source-han-sans-cjk-ja,"Helvetica Neue", Arial, "Hiragino Kaku Gothic ProN", "Hiragino Sans", Meiryo, sans-serif;
  font-style: normal;
  font-weight: 300;
  color: $text--main;
  line-height: 1.8;
  background-color: $bg--white;
}

a {
  text-decoration: none;
  color: $text--main;
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
  @include mq() {
    padding: 40px 0;
  }
}

.text--en {
  font-family: sofia-pro, sans-serif;
}

.text--default {
  font-size: 1.6rem;
  text-align: justify;
  @include mq() {
    font-size: 1.4rem;
  }
}

.title--primary {
  margin-bottom: 40px;
  font-size: 3rem;
  font-weight: 700;
  text-align: center;
  text-transform: uppercase;
  @include mq() {
    margin-bottom: 30px;
    font-size: 2.4rem;
  }
  &::after {
    content: '';
    display: block;
    width: 32px;
    height: 4px;
    margin: 10px auto 0;
    background-color: $text--main;
  }
}
</style>
