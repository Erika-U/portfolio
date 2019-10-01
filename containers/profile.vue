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
      <p>はじめまして。平成8年生まれ、現在23歳のErikaと申します。</p>
      <p>元アパレル店員。接客を約1年半経験後、IT企業に1年半勤務。</p>
      <p>成長が早く、より良いものが次々と生まれるWebの技術に強い魅力を感じ、</p>
      <p>真剣に技術を磨こうと決断。</p>
      <p>2019年5月、勤めていた会社を退職。</p>
      <p>現在は技術力を高めるため、日々Webサイトの制作を行い学びを深めています。</p><br>
      <p>一番直近の大きな目標はWeb系企業に就職すること。</p>
      <p>夢は、UI/UXにこだわったユーザーに愛されるオシャレなサイトを創ること。</p>
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
          {key: '名前',
          value: 'Erika'},
          {key: '生年月日',
          value: '1996/09/01'},
          {key: '性別',
          value: '女性'},
          {key: '住所',
          value: '京都'}
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
      margin-bottom: 50px;
      height: 130px;

      tr {
        margin-bottom: 50px;

      th {
          padding-right: 20px;
          font-size: 14.5px;
        }

      td {
        padding-left: 20px;
          }
        }
      }
    }

    p {
      width: 70%;
      margin: 0 auto;
      margin-bottom: 5px;
    }






</style>
