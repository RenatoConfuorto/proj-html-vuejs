<template>
  <section class="jumbotron">
    <div class="jumbotron-text">
      <h3>We remove the headeache from moving</h3>
      <h2>Move With Ease</h2>
      <p>With our super simple service we can take you from getting a quote, right through to being in your new home with all of your belongings securly packed and safely delivered, even in the rooms of your choice.</p>

      <a href="#" class="btn">Get a free quote now</a>
    </div>
  </section>
</template>

<script>
export default {
  name: 'AppJumbotron',
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.jumbotron{
  text-align: center;
  color: $text-primary-color;
  padding: $main-section-padding;
  background-image: url(../assets/img/avada-movers-movewithease-background-new.jpg);
  background-size: cover;
  background-position: center;

  &-text{
    margin: 0 10rem 0 auto;
    padding: 2rem;
    width: 30%;
    border: 8px solid $brand-primary-color-dark;
    background-color: $brand-primary-color;

    h3{
      text-transform: uppercase;
      font-size: .7rem;
      margin-bottom: 15px;
    }

    h2{
      display: inline-block;
      padding: 0 5px;
      padding-bottom: 1rem;
      margin-bottom: 1rem;
      border-bottom: 2px solid #8fce53;
    }

    p{
      line-height: 1.6;
      margin-bottom: 1rem;
    }
  }
}
</style><style>
