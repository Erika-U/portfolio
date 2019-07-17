<template>
  <h2 class="title">
    {{ title }}
  </h2>
</template>

<script>
  export default {
    name: 'profile',
    props: {
      title: {
        type: String,
        default: ''
      }
    }
  }
</script>
