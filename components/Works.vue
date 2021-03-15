<template>
  <section class="works section__area">
    <div class="inner__main">
      <h2 class="title--primary text--en">Works</h2>
      <ul class="worksList">
        <li v-for="worksList in worksLists" v-bind:key="worksList.id" class="worksList__content">
          <div class="worksList__info">
            <h3 class="worksList__title">{{ worksList.name }}</h3>
            <p class="worksList__period">( {{ worksList.period }} )</p>
            <ul class="worksList__incharge">
              <li v-for="inCharge in worksList.inCharges" class="worksList__incharge_text">{{ inCharge }}</li>
            </ul>
            <ul class="worksList__category">
              <li v-for="category in worksList.categories" class="worksList__category_text">{{ category }}</li>
            </ul>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      worksLists: [
        {
          name: '自社(株式会社CI)コーポレートサイト リニューアル',
          period: '2020年6月〜2020年8月',
          inCharges: [
            'ロゴデザイン案作成',
            '名刺デザイン案作成',
            'Webサイトワイヤーフレーム、デザイン案作成、コーディング'
          ],
          categories: [
            'HTML',
            'CSS',
            'JavaScript',
            'React.js',
            'Photoshop',
            'Illustrator',
            'Adobe XD'
          ]
        },
        {
          name: '教育関連サービスのデザイン',
          period: '2020年5月',
          inCharges: [
            '仕様書を基に、追加開発のデザイン案作成',
          ],
          categories: [
            'Photoshop',
            'Illustrator',
            'Adobe XD'
          ]
        },
        {
          name: '不動産系企業のWebサイト制作',
          period: '2019年12月〜2020年3月',
          inCharges: [
            'Webサイトデザイン、コーディング',
            'WordPressのブランクテーマ(Underscores)を使用したテーマ作成',
          ],
          categories: [
            'HTML',
            'CSS',
            'JavaScript',
            'WordPress',
            'Vagrant',
            'Photoshop',
            'Illustrator',
            'Adobe XD'
          ]
        },
        {
          name: '外国人就職マッチングアプリ開発',
          period: '2019年4月〜2019年11月',
          inCharges: [
            'サービスロゴデザイン',
            'アプリデザイン',
            'サービスのLPサイトデザイン、コーディング',
            'WordPressのブランクテーマ(Underscores)を使用したテーマ作成'
          ],
          categories: [
            'HTML',
            'CSS',
            'JavaScript',
            'WordPress',
            'Vagrant',
            'Photoshop',
            'Illustrator',
            'Adobe XD'
          ]
        },
      ],
    }
  }
}
</script>

<style lang="scss" scoped>
.works .worksList {}

.works .worksList__content {
  display: flex;
  width: 100%;
  height: 100%;
  padding-bottom: 30px;
  margin-bottom: 30px;
  border-bottom: 1px solid $border--gray;
  &:last-child {
    margin-bottom: 0;
    border-bottom: none;
  }
}

.works .worksList__title {
  font-size: 1.6rem;
  font-weight: 500;
}

.works .worksList__period {
  margin-bottom: 15px;
  font-size: 1.2rem;
  font-weight: 300;
}

.works .worksList__incharge {
  margin-bottom: 20px;
  .worksList__incharge_text {
    padding-left: 10px;
    font-size: 1.4rem;
    &::before {
      content: '';
      display: inline-block;
      width: 5px;
      height: 5px;
      margin-right: 8px;
      border: 1px solid $border--black;
      background-color: transparent;
      vertical-align: middle;
    }
    &:last-child {
      margin-bottom: 0;
    }
  }
}

.works .worksList__category {
  display: flex;
  flex-wrap: wrap;
  .worksList__category_text {
    margin: 0 5px 5px 0;
    padding: 0 5px;
    font-size: 1.2rem;
    background-color: $tag--gray;
    border-radius: 2px;
    &:last-child {
      margin-right: 0;
    }
  }
}
</style>
