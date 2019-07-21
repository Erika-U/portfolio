<template>
  <section id="profile" class="profile-wrapper">
    <pageTitle title="profile" />
    <div class="box-wrapper">
      <table>
        <tbody>
          <tr v-for="(contact, index) in contacts" :key="index">
            <th>{{ contact.key }}</th>
            <td>:</td>
            <td>{{ contact.value }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </section>
</template>

<script>
  import pageTitle from '@/components/pageTitle'

  export default {
    name: 'Profile',
    components: {
      pageTitle
    },
    data() {
      return {
        contacts: [
          {key: 'Name',
          value: 'erika'},
          {key: 'Name',
          value: 'erika'}
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
@import '@/assets/styles/_color.scss';
@import '@/assets/styles/_mixin.scss';

  .profile-wrapper {
    @include section;

    table {
      margin: 0 auto;
    }
  }





</style>
