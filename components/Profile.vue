<template>
  <section class="profile section__area">
    <div class="inner__main">
      <h2 class="title--primary">Profile</h2>
      <div class="text__area">
        <p class="text--default">ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。</p>
        <p class="text--default">ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。</p>
        <p class="text--default">ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。ここにはテキストが入ります。</p>
      </div>
    </div>
  </section>
</template>

<script>

</script>

<style lang="scss" scoped>
.profile {
  .title--primary {
    text-align: center;
    &:after {
      margin: 10px auto 0;
    }
  }
}

.text__area {
  .text--default {
    margin-bottom: 30px;
    &:last-child {
      margin-bottom: 0;
    }
  }
}
</style>
