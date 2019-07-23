<template>
  <section id="works" class="works-wrapper">
    <pageTitle title="works" />
    <div class="box-wrapper">
      <div>
        <img src="@/assets/image/work1.png">
        <p>- myPortfolio-</p>
        <p>HTML5, SCSS, Vue.js, Nuxt.js</p>
        <a href="https://github.com/Erika-U/portfolio">git hub</a>
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
        width: 400px;
        height: 600px;
        display: block;
        margin-bottom: 30px;
        max-width: 450px;

      img {
        width: 300px;
        height: 300px;
        }

        a {
          color: darken($main_color, 20%);

          &:hover {
            color: pink;
          }
        }
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
