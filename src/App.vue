<template>
  <div id="app">
    <AppHeader/>

    <main>
      <AppTestimonials/>
    </main>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppTestimonials from "./components/AppTestimonials.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppTestimonials,
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
