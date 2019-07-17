<template>
  <main>
    <section id="top">
      {{ siteName }}
    </section>
    <profile />
    <skills />
    <works />
    <hobbies />
    <other />
  </main>
</template>

<script>
import Profile '@/containers/profile'
import Skills '@/containers/skills'
import Works '@/containers/works'
import Hobbies '@/containers/hobbies'
import Other '@/containers/other'

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
      siteName: `'Erika${'}s Portfolio'`
    }
  }
}
</script>
