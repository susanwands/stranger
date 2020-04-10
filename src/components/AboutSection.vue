<template>
  <div id="about">
    <img alt="Stranger Things" src="../assets/stranger-things_raw.png">
    <p>{{ this.$t('snippets')[1] }}</p>
  </div>
</template>

<script>
export default {
  name: 'about-section',
}
</script>

<style scoped>

#about{
  margin: auto;
  padding-top: 100px;
  width: 90%;
  text-align: center;
}
img{
  padding:1.5rem;
}
</style>
