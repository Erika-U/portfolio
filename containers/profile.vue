<template>
  <section id="profile">
    <pageTitle title="profile" />
    <div>
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
          value: 'erika'}
        ]
      }
    }
  }
</script>
