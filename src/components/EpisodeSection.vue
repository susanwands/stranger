<template>
  <div id="episodes">
    <h2>Episodes</h2>
    <b-table striped hover :items="episodes" :fields="fields" dark responsive></b-table>
  </div>
</template>

<script>
  export default {
    name: 'episode-section',
    computed:{
        episodes() {
            return this.$t('episode-list')
        }
    },
    data() {
      return {
        fields: [
          {
            key: 'season',
            sortable: true
          },
          {
            key: 'name',
            label:'Title',
            sortable: true
          },
          {
            key: 'rating',
            sortable: true,
          }
        ]
      }
    }
  }
</script>

<style scoped>

#episodes{
  margin: auto;
  color: #fff;
  padding-top: 100px;
}

</style>