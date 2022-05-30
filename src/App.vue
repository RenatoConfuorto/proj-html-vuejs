<template>
  <div id="app">
    <div class="up-btn">
      <a href="#up"><i class="fas fa-chevron-up"></i></a>
    </div>
    <AppHeader id="up"/>

    <main>
      <AppTestimonials/>
      <ServiceSolutions/>
      <AppJumbotron/>
      <ReferenceCustomers/>
      <QuoteRequest/>
    </main>

    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppTestimonials from "./components/AppTestimonials.vue";
import ServiceSolutions from "./components/ServiceSolutions.vue";
import AppJumbotron from "./components/AppJumbotron.vue";
import ReferenceCustomers from "./components/ReferenceCustomers.vue";
import QuoteRequest from "./components/QuoteRequest.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppTestimonials,
    ServiceSolutions,
    AppJumbotron,
    ReferenceCustomers,
    QuoteRequest,
    AppFooter,
  }
}
</script>

<style lang="scss">
@import "style/common.scss";
@import "style/variables.scss";
@import '~@fortawesome/fontawesome-free/css/all.min.css';

.up-btn{
  background-color: #6b6b6b;
  position: fixed;
  bottom: 0;
  right: 30px;
  width: 2.5rem;
  height: 2rem;
  line-height: 2rem;
  text-align: center;
  border-top-right-radius: 5px;
  border-top-left-radius: 5px;

  i{
    color: $text-primary-color;
    padding: .4rem;
  }
}
</style>
