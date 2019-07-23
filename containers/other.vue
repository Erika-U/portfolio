<template>
  <section id="other" class="other-wrapper">
    <pageTitle title="other" />
    <div class="box-wrapper">
      <div v-for="(contact, index) in contacts" :key="index">
        <p class="other_title">{{ contact.key }}</p>
        <p class="other_data">{{ contact.value }}</p>
      </div>
    </div>
  </section>
</template>

<script>
  import pageTitle from '@/components/pageTitle'

  export default {
    name: 'Other',
    components: {
      pageTitle
    },
    data() {
      return {
        contacts: [
          {key: '- 注目している技術 -',
          value: 'アルゴレイヴ 、Webアニメーション'},
          {key: '- webに興味を持ったきっかけ -',
          value: 'デザインの流行があり、技術の進化のスピードが早く、ユーザーの使いやすさが求められるなど、他にも多くの要素で構成されていて奥が深いと思ったから。'},
          {key: '- 自覚している性格 -',
          value: 'とにかく真面目。行動力と根性には自信あり。好奇心旺盛で新しいことが好き。少し飽き性...。人と関わることが好きで、情に厚い。前向きで何事も最後まで諦めない粘り強さがある。少し突っ走りやすい。'}
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import '@/assets/styles/_color.scss';
  @import '@/assets/styles/_mixin.scss';

  .other-wrapper {
    @include section;


    p {
    margin: 0 auto;
    max-width: 80%;
    }

    .other_title {
      font-size: 20px;
      margin-bottom: 15px;
    }
    .other_data {
      width: 400px;
      margin-bottom: 70px;
      }
    }
</style>
