<template>
  <main>
    <section id="top">
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
