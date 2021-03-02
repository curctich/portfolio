<template>
  <section class="works section__area">
    <div class="inner__main">
      <h2 class="title--primary">Works</h2>
      <ul class="works__list">
        <li v-for="worksList in worksLists" v-bind:key="worksList.id" class="works__list_unit">
          <h3 class="works__list_title">
            {{ worksList.name }}
            <span>( {{ worksList.period }} )</span>
          </h3>
          <ul class="works__list_content">
            <li v-for="inCharge in worksList.inCharges">{{ inCharge }}</li>
          </ul>
          <ul class="works__list_info">
            <li v-for="category in worksList.categories">{{ category }}</li>
          </ul>
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
          name: '外国人就職マッチングアプリ開発',
          period: '2019年4月〜2019年11月',
          inCharges: [
            'サービスロゴデザイン',
            'アプリデザイン',
            'サービスのLPサイトデザイン、コーディング',
            'WordPressのブランクテーマを使用したテーマ作成'
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
          name: '不動産系企業のWebサイト制作',
          period: '2019年12月〜2020年3月',
          inCharges: [
            'Webサイトデザイン、コーディング',
            'WordPressのブランクテーマを使用したテーマ作成',
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
          name: '自社サイト リニューアル',
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
        }
      ],
    }
  }
}
</script>

<style lang="scss" scoped>
.works__list_unit {
  margin-bottom: 30px;
  &::after {
    content: '';
    display: block;
    width: 100%;
    height: 1px;
    margin-top: 30px;
    background-color: #dadada;
  }
  &:last-child {
    margin-bottom: 0;
    &::after {
      display: none;
    }
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
}

.works__list_content {
  margin-bottom: 20px;
  li {
    padding-left: 10px;
    font-size: 1.4rem;
    line-height: 1.8;
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
  flex-wrap: wrap;
  li {
    margin: 0 5px 5px 0;
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
