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
          'aaaaaa',
          'aaaaaa',
          'aaaaaa',
          'aaaaaa',
          'aaaaaa',
          'aaaaaa'
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
  }
</style>
