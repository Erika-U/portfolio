<template>
  <section id="skills" class="skills-wrapper">
    <pageTitle title="skills" />
    <div class="box-wrapper">
    <ul>
      <li v-for="skill in skills">{{ skill }}</li>
    </ul>
    </div>
  </section>
</template>

<script>
  import pageTitle from '@/components/pageTitle'

  export default {
    name: 'Skills',
    components: {
      pageTitle
    },
    data() {
      return {
        skills: [
          '・ HTML5&CSS3',
          '・ Sass', 
          '・ PHP',
          '・ Laravel',
          '・ JavaScript',
          '・ Vue.js',
          '・ Docker',
          '・ MySQL',
          '・ Git',
          '・ Redmine',
          '・ slack'
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import '@/assets/styles/_color.scss';
  @import '@/assets/styles/_mixin.scss';

  .skills-wrapper {
    @include section;
    @include content-list(33.3%);

    li {
      margin-bottom: 20px;
    }
  }


</style>
