<template>
  <div id="app">
    <AppHeader/>

    <main>
      <AppTestimonials/>
      <ServiceSolutions/>
      <AppJumbotron/>
    </main>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppTestimonials from "./components/AppTestimonials.vue";
import ServiceSolutions from "./components/ServiceSolutions.vue";
import AppJumbotron from "./components/AppJumbotron.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppTestimonials,
    ServiceSolutions,
    AppJumbotron,
  }
}
</script>

<style lang="scss">
@import "style/common.scss";
@import "style/variables.scss";
@import '~@fortawesome/fontawesome-free/css/all.min.css';


#app{
  color: black;
}
</style>
