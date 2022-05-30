<template>
  <section class="main-cnt-section">
    <div class="text-container">
      <h2>Request A Free Quote</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, suscipit provident labore sunt aliquid nulla tempore, officiis accusamus qui temporibus doloremque voluptate dolor ex. Blanditiis ab nulla aliquid maxime nam?</p>

      <a href="#" class="btn">Click here</a>
    </div>

  </section>
</template>

<script>
export default {
naeme: 'QuoteRequest',
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.main-cnt-section{
  background-image: url(../assets/img/avada-movers-request-quote-background.jpg);
  background-size: cover;
  background-position: center;

  .text-container{
    width: 50%;
    margin: 0 auto;
    
    p{
      color: $text-secondary-color;
      margin-bottom: 2rem;
    }
  }
}

</style>
