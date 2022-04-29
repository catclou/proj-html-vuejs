<template>
  <div id="app">
    <!-- <h1 class="text-success">Titolo di prova <i class="fa-solid fa-circle-check"></i></h1> -->
    <HeaderComp/>
    <HeroFirst/>
    <MeetSection/>
    <TopNotch/>
    <OurWork/>
    <OurPlans/>
    <OurNews/>
    <OurClients/>
    <FreeConsultation/>
    <FooterComp/>
  </div>
</template>

<script>
import "bootstrap"
// import HelloWorld from './components/HelloWorld.vue'
import HeaderComp from './components/HeaderComp.vue'
import HeroFirst from './components/HeroFirst.vue'
import MeetSection from './components/MeetSection.vue'
import TopNotch from './components/TopNotch.vue'
import OurWork from './components/OurWork.vue'
import OurPlans from './components/OurPlans.vue'
import OurNews from './components/OurNews.vue'
import OurClients from './components/OurClients.vue'
import FreeConsultation from './components/FreeConsultation.vue'
import FooterComp from './components/FooterComp.vue'


export default {
  name: 'App',
  components: {
    HeaderComp,
    HeroFirst,
    MeetSection,
    TopNotch,
    OurWork,
    OurPlans,
    OurNews,
    OurClients,
    FreeConsultation,
    FooterComp
  }
}
</script>

<style lang="scss">
@import "bootstrap/dist/css/bootstrap.min.css";

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
