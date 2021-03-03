<template>
  <section class="career section__area">
    <div class="inner__main">
      <h2 class="title--primary text--en">Career</h2>
      <ol class="timeline">
        <li v-for="careerTimeline in careerTimelines" v-bind:key="careerTimeline.id" class="timeline__unit">
          <time class="timeline__title">{{ careerTimeline.year }}</time>
          <div class="timeline__content">
            <p v-for="careerTimelineText in careerTimeline.careerTimelineTexts" class="timeline__content_text">{{ careerTimelineText }}</p>
          </div>
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
.career .timeline {}

.career .timeline__unit {
  position: relative;
  padding: 0 0 20px 20px;
  &::before {
    content: '';
    position: absolute;
    top: 6px;
    left: 0;
    z-index: 2;
    display: inline-block;
    width: 10px;
    height: 10px;
    border: 2px solid #212121;
    border-radius: 50%;
    background-color: #fff;
  }
  &::after {
    content: '';
    position: absolute;
    top: 6px;
    left: 4px;
    display: inline-block;
    width: 1px;
    height: 100%;
    border: 1px solid #ebebeb;
  }
  &:last-child {
    &::after {
      display: none;
    }
    .timeline__content {
      &::after {
        display: none;
      }
    }
  }
}

.career .timeline__title {
  display: inline-block;
  width: 100%;
  margin-bottom: 15px;
  font-size: 1.6rem;
  font-weight: 500;
}
.career .timeline__content {
  &::after {
    content: '';
    display: inline-block;
    width: 100%;
    height: 100%;
    margin-top: 30px;
    border-bottom: 2px dotted #ebebeb;
  }
}

.career .timeline__content_text {
  font-size: 1.4rem;
  line-height: 1.8;
}
</style>
