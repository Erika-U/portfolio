<template>
  <header>
    <div class="link">
      <nuxt-link v-scroll-to="'#top'" to>
        Top
      </nuxt-link>
      <nuxt-link v-scroll-to="'#profile'" to>
        Profile
      </nuxt-link>
      <nuxt-link v-scroll-to="'#skills'" to>
        Skills
      </nuxt-link>
      <nuxt-link v-scroll-to="'#works'" to>
        Works
      </nuxt-link>
      <nuxt-link v-scroll-to="'#hobbies'" to>
        Hobbies
      </nuxt-link>
      <nuxt-link v-scroll-to="'#other'" to>
        Other
      </nuxt-link>
    </div>
  </header>
</template>
<script>
  export default {
    name: 'MyHeader'
  }
</script>
<style lang="scss" scoped>
@import '@/assets/styles/_color.scss';
@import '@/assets/styles/_mixin.scss';

  .link {
    display: flex;
    width: 100%;
    text-align: center;
    margin: 0 auto;
    justify-content: center;
    align-items: center;
    height: 80px;
    position: fixed;
    background-color: white;
    box-shadow: 0 0 5px 0 rgba(0, 0, 0, 0.3);


    a {
      width: 150px;
      height: 100%;
      padding-top: 30px;
      text-decoration: none;
      transition: all 0.3s;
      cursor: pointer;
      user-select: none;
      color: darken($main_color, 20%);

      &:hover {
        background-color: lighten(pink, 5%);
      }
    }
  }
</style>
