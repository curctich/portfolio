<template>
  <section class="works section__area">
    <div class="inner__main">
      <h2 class="title--primary">Works</h2>

      <ul class="works__list">
        <li class="works__list_unit">
          <h3 class="works__list_title">
            外国人就職マッチングアプリ開発
            <span>( 2019年4月〜2019年11月 )</span>
          </h3>
          <div class="works__list_content">
            <p class="text--default">担当内容</p>
            <ul>
              <li>サービスロゴデザイン</li>
              <li>アプリデザイン</li>
              <li>サービスのLPサイトデザイン、コーディング</li>
              <li>WordPressのブランクテーマを使用したテーマ作成</li>
            </ul>
          </div>
          <ul class="works__list_info">
            <li>HTML</li>
            <li>CSS</li>
            <li>Javascript</li>
            <li>WordPress</li>
            <li>Vagrant</li>
          </ul>
        </li>

      </ul>
    </div>
  </section>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
.works__list_unit {
  margin-bottom: 40px;
  &:last-child {
    margin-bottom: 0;
  }
}

.works__list_title {
  margin-bottom: 15px;
  font-size: 1.6rem;
  span {
    display: block;
    font-size: 1.2rem;
    font-weight: normal;
  }
  &::after {
    content: '';
    display: block;
    width: 100%;
    height: 1px;
    margin-top: 15px;
    background-color: #dadada;
  }
}

.works__list_content {
  margin-bottom: 20px;
  p {
    margin-bottom: 8px;
    &::before {
      content: '';
      display: inline-block;
      width: 6px;
      height: 6px;
      margin-right: 8px;
      background-color: #212121;
      vertical-align: middle;
    }
  }
  ul li {
    padding-left: 10px;
    margin-bottom: 5px;
    font-size: 1.4rem;
    &::before {
      content: '';
      display: inline-block;
      width: 5px;
      height: 5px;
      margin-right: 8px;
      border: 1px solid #212121;
      background-color: transparent;
      vertical-align: middle;
    }
    &:last-child {
      margin-bottom: 0;
    }
  }
}

.works__list_info {
  display: flex;
  li {
    margin: 0 5px 0 5px;
    padding: 0 5px;
    font-size: 1.2rem;
    background-color: #f2f2f2;
    border-radius: 2px;
    &:last-child {
      margin-right: 0;
    }
  }
}
</style>
