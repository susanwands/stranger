<template>
  
    <b-container id="app" fluid>
      <b-row>
        <TopNav/>
      </b-row>
      <b-row>
        <b-col>
        <AboutSection id="about" msg="If you're not a Stranger Things fan yet ... you will be"/>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <EpisodeSection/>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <FunFactsSection msg="If you're not a Stranger Things fan yet ... you will be"/>
        </b-col>
      </b-row>
      <b-row>
          <GallerySection/>
      </b-row>
      <b-row>
        <footer>
          <p>Thanks for watching : ) - Susan Wands </p>
        </footer>
      </b-row>
    </b-container>

</template>

<script>
import TopNav from './components/TopNav.vue'
import AboutSection from './components/AboutSection.vue'
import EpisodeSection from './components/EpisodeSection.vue'
import FunFactsSection from './components/FunFactsSection.vue'
import GallerySection from './components/GallerySection.vue'

export default {
  name: 'App',
  components: {
    TopNav,
    AboutSection,
    EpisodeSection,
    FunFactsSection,
    GallerySection
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Merriweather&family=Montserrat&display=swap');
#app {
  font-family: Montserrat, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #fff;
  background-color: #000;
  height: min-content;

}

h1, h2, h3 {
  font-family: Merriweather, serif;
  font-variant:small-caps;
}

footer{
  width: 100%;
  text-align: center;
  background-color: #343a40;
  padding: 1rem;
 

}


</style>
