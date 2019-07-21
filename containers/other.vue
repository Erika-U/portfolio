<template>
  <section id="other">
    <pageTitle title="other" />
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
    name: 'Other',
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
