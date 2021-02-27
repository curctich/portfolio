<template>
  <footer>
    <div class="section__area">
      <div class="inner__main">
        <h2 class="title--primary">Links</h2>
        <ul class="footer__links">
          <li class="footer__links_item">
            <a href="https://github.com/curctich" target="_blank">Github</a>
          </li>
          <li class="footer__links_item">
            <a href="mailto:sieeya.bp@gmail.com">sieeya.bp@gmail.com</a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  background-color: #212121;
  .title--primary {
    color: #fafafa;
    &::after {
      background-color: #fafafa;
    }
  }
}
.footer__links {
  display: flex;
}
.footer__links_item {
  font-size: 1.6rem;
  font-weight: bold;
  transition: all 0.5s;
  a {
    color: #fafafa;
  }
  &::after {
    content: '・';
    padding: 0 10px;
    color: #fafafa;
  }
  &:last-child {
    &::after {
      display: none;
    }
  }
  &:hover {
    opacity: 0.5;
  }
}
</style>
