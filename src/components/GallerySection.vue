<template>
  <div id="gallery-section">
    <b-row>
        <b-col>
           <h2>Gallery</h2>
        </b-col>
    </b-row>
   <div id="gallery">
    <figure
         v-for="(item ,i) in gallery"
         :key="i">
      <img :src="item.src">
      <figcaption>{{item.text}}</figcaption>
    </figure>
  </div>
  </div>
</template>

<script>
export default {
    name: 'gallery-section',
    computed:{
        gallery() {
            return this.$t('gallery')
        }
    }
}
</script>

<style scoped>
#gallery-section{
    width: 100%;
    margin: auto;
    padding: 1rem;
    padding-top: 100px;
}
#gallery{
  display: flex;
  width: 900px;
  margin: auto;
  justify-content: space-between;
  flex-wrap: wrap;
  background-color: #000;
  padding: 1rem;
}
figure{
  width: 400px;
  height: 500px;
  margin: 8px 0;
  border: 1px solid #777;
  padding: 8px;
  box-sizing: border-box;
  background-color: #fff;
}
figure img{
  width: 100%;
  height: 80%
}
figure figcaption{
  text-align: center;
  padding: 8px 4px;
  color:#000;
}
</style>
