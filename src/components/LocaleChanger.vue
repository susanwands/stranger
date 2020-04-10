<template>
  <b-nav-form right>
    <b-form-group label="Lang:" label-for="locale-input">
      <b-form-select v-model="$i18n.locale" size="sm" id="locale-input">
      <b-form-select-option v-for="(lang, i) in langs" :key="`Lang${i}`" :value="lang">{{ lang }}</b-form-select-option>
      </b-form-select>
    </b-form-group>
  </b-nav-form>
</template>

<script>
export default {
  name: 'locale-changer',
  data () {
    return { langs: ['en_US', 'la_PG'] }
  }
}
</script>
<style scoped>

</style>