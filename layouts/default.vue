<template>
  <div>
    <myheader />
    <nuxt />
  </div>
</template>
<script>
  import myheader from '@/components/myheader'

  export default {
    components: {
      myheader
    }
  }
</script>

<style>
html {
  font-family: 'Julius Sans One';
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
</style>
