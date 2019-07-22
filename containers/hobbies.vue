<template>
  <section id="hobbies" class="hobbies-wrapper">
    <pageTitle title="hobbies" />
    <div class="box-wrapper">
      <ul>
        <li v-for="hobbie in hobbies">{{ hobbie }}</li>
      </ul>
    </div>
  </section>
</template>

<script>
  import pageTitle from '@/components/pageTitle'

  export default {
    name: 'Hobbies',
    components: {
      pageTitle
    },
    data() {
      return {
        hobbies: [
          '・ 麻雀',
          '・ 卓球',
          '・ ヴァイオリン',
          '・ カラオケ',
          '・ 音楽鑑賞',
          '・ ケーキを求めてカフェ巡り',
          '・ ファッション/メイク',
          '・ イラスト制作',
          '・ 読書',
          '・ 猫を愛でる',
          '・ 色やデザインの勉強',
          '・ オシャレなWebサイト徘徊'
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import '@/assets/styles/_color.scss';
  @import '@/assets/styles/_mixin.scss';

  .hobbies-wrapper {
    @include section;
    @include content-list(50%);

    li {
      margin-bottom: 20px;
    }
  }
</style>
