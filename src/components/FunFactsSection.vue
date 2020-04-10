<template>
  <div id="fun-facts">
    <h2>Fun Facts</h2>
     <b-row class="fact">
        <b-col>
           <h3>{{ this.$t('heading') }}</h3>
           <p>{{ this.$t('snippets')[2] }}</p>
           <p>{{ this.$t('description')}}</p>
        </b-col>
    </b-row>

    <b-row class="fact">
        <b-col>
           <h3>Take A Tour</h3>
           <p>You can find plenty of sites around town... <q>{{ this.$t('snippets')[0] }}</q></p>
           
           <ul>
               <li  v-for="(item ,i) in locations" :key="i">{{item}}</li>
           </ul>
           
           <p><q>{{ this.$t('quote').text }} </q> - {{ this.$t('quote').author }}</p>
        </b-col>
    </b-row>
   
  </div>
</template>

<script>
export default {
    name: 'fun-facts-section',
    computed:{
        locations() {
            return this.$t('locations')
        }
    }
}
</script>

<style scoped>

#fun-facts{
    margin: auto;
    padding-top: 100px;
}
.fact{
    width: 90%;
    padding-top: 2rem;
    margin: auto;
}
.fact h3 {
    color: lightgray;
}
</style>