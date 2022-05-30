<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <div class="footer-col">
          <h3>About</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Dignissimos magni, nulla natus sequi ipsa rem?
          </p>
          <img src="../assets/img/avada-movers-logo.png" alt="Avada Movers">
        </div>

        <div class="footer-col" v-for="(item, index) in footerNavList" :key="index">
          <h3>{{ item.listTitle }}</h3>
          <ul>
            <li
            v-for="element in item.listElements"
            :key="element.id"
            :class="{active : activeElement == element.id}"
            >
              <a :href="element.url">{{ element.text }}</a>
            </li>
          </ul>
        </div>

      </div>
    </div>
    <div class="footer-bottom">
      <div class="container-small">

      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'AppFooter',
  data(){
    return{
      activeElement: 0,
      footerNavList: [
        {
          listTitle: 'avada movers',
          listElements: [
            {
              url: '#',
              text: 'home',
              id: 0,
            },
            {
              url: '#',
              text: 'rates',
              id: 1,
            },
            {
              url: '#',
              text: 'testimonials',
              id: 2,
            },
            {
              url: '#',
              text: 'blog',
              id: 3,
            },
            {
              url: '#',
              text: 'free quote',
              id: 4,
            },
          ]
        },
        {
          listTitle: 'recent posts',
          listElements: [
            {
              url: '#',
              text: 'heading out to college?',
              id: 5,
            },
            {
              url: '#',
              text: 'Moving youtìr business?',
              id: 6,
            },
            {
              url: '#',
              text: 'outstanding quality',
              id: 7,
            },
            {
              url: '#',
              text: 'cost of moving',
              id: 8,
            },
            {
              url: '#',
              text: 'best moving tips',
              id: 9,
            },
          ]
        },

      ],
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
footer{
  background-color: $brand-primary-color;
  padding-top: 10px;
  
  .footer-top{
    background-color: white;
    padding: 3rem 0;

    .container{
      display: flex;

      .footer-col{
        width: calc(100% / 3);
        padding: 0 1rem;

        h3{
          text-transform: uppercase;
          font-size: 1rem;
          margin-bottom: 1.5rem;
        }

        p{
          line-height: 1.6;
          margin-bottom: 2rem;
          font-size: .8rem;
        }

        img{
          width: 50%;
          height: auto;
        }

        //liste
        ul{
          list-style-type: none;

          li{
            line-height: 2.5;
            text-transform: capitalize;
            font-size: .8rem;

            &::before {
              content: ">";
              padding-right: 3px;
            }

            a{
              text-decoration: none;
              color: $text-secondary-color-dark;
            }

            &.active{

              a{
                color: $brand-primary-color;
              }
            }
          }
        }
      }
    }

  }

  .footer-bottom{
    padding: 1rem 0;

  }
}

</style>style>
