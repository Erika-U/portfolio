<template>
  <header>
    <div class="link">
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


    a {
      width: 150px;
    }
  }
</style>
