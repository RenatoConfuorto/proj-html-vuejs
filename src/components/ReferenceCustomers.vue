<template>
  <section class="main-cnt-section container">
    <h3>Happy customers</h3>
    <h2>Testimonials</h2>
    <div class="card-container">
      <div
      class="card"
      v-for="(element, index) in cardCnt"
      :key="index"
      >
        <div class="img-wrapper">
          <img :src="require(`../assets/img/${element.img}`)" :alt="element.name">
        </div>

        <div class="card-text">
          <h3>{{ element.name }}</h3>
          <p>{{ element.text }}</p>
        </div>
      </div>
    </div>

    <a href="#" class="btn">Read more testimonials</a>
  </section>
</template>

<script>
export default {
  name: 'ReferenceCustomers',
  data(){
    return{
      cardCnt: [
        {
          img: 'avada-movers-johndoe-final.jpg',
          name: 'John Doe',
          text: '"Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit recusandae autem eaque, veritatis odio pariatur ipsa adipisci non neque ipsam corrupti assumenda molestias, deleniti voluptate quo animi blanditiis tempore qui?"',
        },
        {
          img: 'avada-movers-janedoe-final.jpg',
          name: 'Jane Doe',
          text: '"Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit recusandae autem eaque, veritatis odio pariatur ipsa adipisci non neque ipsam corrupti assumenda molestias, deleniti voluptate quo animi blanditiis tempore qui?"',
        },
        {
          img: 'avada-movers-johnsmith-final.jpg',
          name: 'John Smith',
          text: '"Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit recusandae autem eaque, veritatis odio pariatur ipsa adipisci non neque ipsam corrupti assumenda molestias, deleniti voluptate quo animi blanditiis tempore qui?"',
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
    margin-bottom: 2rem;

    .card{

      .img-wrapper{
        border-radius: 50%;
        overflow: hidden;
      }

      &-text{

        p{
          font-style: italic;
        }
      }
    }

  }
}

</style><style>

