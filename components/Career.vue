<template>
  <section class="career section__area">
    <div class="inner__main">
      <h2 class="title--primary">Career</h2>
      <ol class="career__timeline">
        <li v-for="careerTimeline in careerTimelines" v-bind:key="careerTimeline.id" class="career__timeline_unit">
          <time class="career__timeline_title">{{ careerTimeline.year }}</time>
          <p v-for="careerTimelineText in careerTimeline.careerTimelineTexts" class="career__timeline_text">{{ careerTimelineText }}</p>
        </li>
      </ol>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      careerTimelines: [
        {
          year: '2020',
          careerTimelineTexts: [
            '株式会社CI 退社'
          ]
        },
        {
          year: '2019',
          careerTimelineTexts: [
            '株式会社CI 入社',
            'デジタルハリウッド大阪校 Webデザイナー専攻 修了'
          ]
        },
        {
          year: '2018',
          careerTimelineTexts: [
            'デジタルハリウッド大阪校 Webデザイナー専攻 入学',
            '株式会社Lovin 退社'
          ]
        },
        {
          year: '2012',
          careerTimelineTexts: [
            '株式会社Lovin 入社',
            '株式会社ミスティー・コレクション 退社'
          ]
        },
        {
          year: '2010',
          careerTimelineTexts: [
            '株式会社ミスティー・コレクション 入社'
          ]
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.career__timeline {}

.career__timeline_unit {
  position: relative;
  padding-left: 20px;
  margin-bottom: 30px;
  &::before {
    content: '';
    top: 6px;
    left: 0;
    position: absolute;
    display: inline-block;
    width: 10px;
    height: 10px;
    border: 2px solid #212121;
    background-color: transparent;
  }
  &::after {
    content: '';
    position: absolute;
    top: 0;
    left: 4px;
    display: inline-block;
    width: 1px;
    height: 100%;
    margin-top: 24px;
    border: 1px solid #ebebeb;
  }
}

.career__timeline_title {
  display: inline-block;
  margin-bottom: 10px;
  font-size: 1.6rem;
}

.career__timeline_text {
  font-size: 1.4rem;
  line-height: 1.8;
}
</style>
