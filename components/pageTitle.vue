<template>
  <h2 class="title">
    {{ title }}
  </h2>
</template>

<script>
  export default {
    name: 'PageTitle',
    props: {
      title: {
        type: String,
        default: ''
      }
    }
  }
</script>
