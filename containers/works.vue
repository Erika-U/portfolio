<template>
  <section id="works" class="works-wrapper">
    <pageTitle title="works" />
    <div class="box-wrapper">
      <div v-for="work in works">
        <img v-bind:src='work.image'>
        <p>{{ work.title }}</p>
        <p>{{ work.desc }}</p>
        <a v-bind:href="work.url" target="_blank">git hub</a>
      </div>
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
          {image: require('@/assets/image/work1.png'),
           title: '- myPortfolio-',
           desc: 'HTML5, SCSS, Vue.js, Nuxt.js',
           url: 'https://github.com/Erika-U/portfolio'},
           {image: require('@/assets/image/work2.png'),
            title: '-TODO List-',
            desc: 'Docker, Laravel, SCSS, Vue.js, Vuex',
            url: 'https://github.com/Erika-U/todo'},
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
        margin-bottom: 75px;
        display: block;

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



</style>
