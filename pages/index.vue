<template>
  <main>
    <section id="top" class="top-wrapper">
      <h1>{{ siteName }}</h1>
    </section>
    <profile />
    <skills />
    <works />
    <hobbies />
    <other />
  </main>
</template>

<script>
import Profile from '@/containers/profile'
import Skills from '@/containers/skills'
import Works from '@/containers/works'
import Hobbies from '@/containers/hobbies'
import Other from '@/containers/other'

export default {
  name: 'Top',
  components: {
    Profile,
    Skills,
    Works,
    Hobbies,
    Other
  },
  data() {
    return {
      siteName: 'Erika\'s Portfolio'
    }
  }
}
</script>

<style lang="scss" scoped>
  @import '@/assets/styles/_color.scss';
  @import '@/assets/styles/_mixin.scss';

  .top-wrapper {
    text-align: center;
    height: 100vh;
    background-color: $main_color;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 120px;

    h1 {
      font-family: Julius Sans One;
      font-size: 80px;
      color: white;
      user-select: none;
    }

    @media screen and (max-width: 1024px) {
      h1 {
        font-size: 50px;
      }
    }

    @media screen and (max-width: 555px) {
      h1 {
        font-size: 40px;
      }
    }
  }

</style>
