<template>
  <div id="app">
    <AppHeader/>

    <main>
      <AppTestimonials/>
      <ServiceSolutions/>
      <AppJumbotron/>
      <ReferenceCustomers/>
      <QuoteRequest/>
    </main>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppTestimonials from "./components/AppTestimonials.vue";
import ServiceSolutions from "./components/ServiceSolutions.vue";
import AppJumbotron from "./components/AppJumbotron.vue";
import ReferenceCustomers from "./components/ReferenceCustomers.vue";
import QuoteRequest from "./components/QuoteRequest.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppTestimonials,
    ServiceSolutions,
    AppJumbotron,
    ReferenceCustomers,
    QuoteRequest,
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
