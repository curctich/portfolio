<template>
  <div class="mv">
    <div class="mv__title_wrapper">
      <h1 class="mv__title text--en">portfolio<span>Saori Yajima</span></h1>
    </div>
  </div>
</template>

<script>

</script>

<style lang="scss" scoped>
.mv {
  position: relative;
  width: 100%;
  height: 500px;
}
.mv .mv__title_wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}

.mv .mv__title {
  position: relative;
  padding: 6%;
  font-size: 5rem;
  text-align: center;
  text-transform: uppercase;
  span {
    display: block;
    margin-top: 15px;
    font-size: 1.8rem;
    text-transform: none;
    color: #bababa;
  }
  &::before,
  &::after {
    content: '';
    position: absolute;
    display: inline-block;
    opacity: 0;
    animation: mv-border ease-in-out 0.8s 0.2s forwards;
  }
  &::before {
    top: 0;
    left: 0;
    border-left: 2px solid #212121;
    border-top: 2px solid #212121;
  }
  &::after {
    bottom: 0;
    right: 0;
    border-right: 2px solid #212121;
    border-bottom: 2px solid #212121;
  }
}

@keyframes mv-border {
  0% {
    width: 0;
    height: 0;
    opacity: 1;
  }
  100% {
    width: 100%;
    height: 100%;
    opacity: 1;

  }
}
</style>
