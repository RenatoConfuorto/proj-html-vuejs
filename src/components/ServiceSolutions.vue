<template>
  <section class="main-cnt-section container">
    <h3>We are professionals</h3>
    <h2>Full-Service Solution</h2>
<!-- ..\assets\img -->
    <div class="card-container">
      <div
      class="card"
      v-for="(element, index) in cardCnt"
      :key="index"
      >
        <div class="img-wrapper">
          <img :src="require(`../assets/img/${element.img}`)" alt="element.title">
        </div>

        <div class="card-text">
          <h3>{{ element.title }}</h3>
          <p>{{ element.text }}</p>

          <a href="#" class="btn">Read More</a>
        </div>

      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ServiceSolutions',
  data(){
    return{
      cardCnt: [
        {
          img: 'avada-movers-serviceonephoto-final.jpg',
          title: 'Two Man Teams',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt animi architecto dolore maxime quisquam molestias dolores nobis natus! Explicabo, alias voluptas. Facilis autem magni iste facere nemo veritatis minima nesciunt.',
        },
        {
          img: 'avada-movers-servicetwophoto-final.jpg',
          title: 'We Do All The Lifting',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt animi architecto dolore maxime quisquam molestias dolores nobis natus! Explicabo, alias voluptas. Facilis autem magni iste facere nemo veritatis minima nesciunt.',
        },
        {
          img: 'avada-movers-servicethreephoto-final.jpg',
          title: 'Coast To Coast',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt animi architecto dolore maxime quisquam molestias dolores nobis natus! Explicabo, alias voluptas. Facilis autem magni iste facere nemo veritatis minima nesciunt.',
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.main-cnt-section{

  .card-container{

    .card{
      background-color: $background-color-section;

      &-text{
        background-color: white;
        
        p{
          margin-bottom: 15px;
        }
      }
    }
  }
}

</style>>