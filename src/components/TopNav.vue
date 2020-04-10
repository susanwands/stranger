<template>
  
    <b-navbar class="top-nav" toggleable="lg" type="dark" variant="dark" fixed="top">
         <b-navbar-brand href="#">
            <img src="../assets/stranger-things_raw.png" id="brand-image" class="d-inline-block align-top" alt="Stranger Things">
        </b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
            <b-nav-item href="#about">About</b-nav-item>
            <b-nav-item href="#episodes">Episodes</b-nav-item>
            <b-nav-item href="#fun-facts">Fun Facts</b-nav-item>
            <b-nav-item href="#gallery-section">Gallery</b-nav-item>
        </b-navbar-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
            <LocaleChanger/>
        </b-navbar-nav>
        </b-collapse>
    </b-navbar>
   
</template>

<script>
import LocaleChanger from './LocaleChanger.vue'

export default {
  name: 'top-nav',
    components: {
        LocaleChanger
    }
}
</script>
<style scoped>
.top-nav{
    width: 100%;
}
#brand-image{
    max-height: 30px;
}
</style>