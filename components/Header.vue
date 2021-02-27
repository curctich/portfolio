<template>
  <header>
    <div class="inner__main header__wrapper">
      <nav>
        <ul class="header__nav">
          <li class="header__nav_item">
            <nuxt-link to="/">home</nuxt-link>
          </li>
          <li class="header__nav_item">
            <nuxt-link to="/works">works</nuxt-link>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.header__wrapper {
  display: flex;
  justify-content: flex-end;
}
.header__nav {
  display: flex;
}
.header__nav_item {
  padding: 15px;
  font-size: 1.6rem;
  font-weight: bold;
  text-transform: uppercase;
  transition: all 0.5s;
  &:hover {
    opacity: 0.5;
  }
}
</style>
