<template>
  <section id="works" class="works-wrapper">
    <pageTitle title="works" />
    <div class="box-wrapper">
      <div>
        <p>イメージ部分</p>
        <p>説明部分</p>
      </div>
      <div></div>
      <div></div>
    </div>
  </section>
</template>

<script>
  import pageTitle from '@/components/pageTitle'

  export default {
    name: 'Works',
    components: {
      pageTitle
    },
    data() {
      return {
        works: [
          {key: 'Name',
          value: 'erika'}
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import '@/assets/styles/_color.scss';
  @import '@/assets/styles/_mixin.scss';

  .works-wrapper {
    @include section;

    .box-wrapper {
      div {
        margin: 0 auto;
        width: 300px;
        height: 300px;
        background-color: pink;
        display: block;
        margin-bottom: 30px;
        max-width: 450px;
      }
    }
  }


  @media(min-width:   1000px) {
    div {
      padding-left: 20px;
      padding-right: 20px;
      display: flex;
      margin: 0 auto;
    }
  }

  @media(min-width:   1200px) {
    div {
      padding-left: 20px;
      padding-right: 20px;
      display: flex;
      margin: 0 auto;
      max-width: 80%;
    }
  }

</style>
