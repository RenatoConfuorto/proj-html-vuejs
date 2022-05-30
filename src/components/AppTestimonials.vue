<template>
  <section class="main-cnt-section">
    <h3>Headhache free</h3>
    <h2>Award Winning <br>Moving Company</h2>
    <div class="text-container">
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ut quidem molestias sequi quo odit enim ducimus sint fugiat quaerat eius iure, vitae ipsum, voluptatum, laboriosam quae praesentium minima sit saepe!</p>
    </div>
    <a href="#" class="btn">Read our testimonials</a>
  </section>
</template>

<script>
export default {
  name: 'AppTestimonials',
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.main-cnt-section{
  background-color: $background-color-section;

  .text-container{
    width: 50%;
    margin: 0 auto;
    margin-bottom: 40px;
  }
}

</style>