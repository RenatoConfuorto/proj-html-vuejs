<template>
  <header>

    <div class="cta">
      <div class="container">
        <div class="call-section">
          <i class="fas fa-phone-alt"></i>
          Call us for a Free Quote 1.800.555.6789
        </div>

        <SocialLinks/>
      </div>
    </div>

      <div class="navbar">
        <div class="container">
          <div class="logo-wrapper">
            <img src="../assets/img/avada-movers-logo.png" alt="Avada Movers">
          </div>

        <nav>
          <ul class="line-list">
            <li v-for="(element, index) in navElements" :key="index">
              <a :href="element.url" :class="{active: index == activeElement}">{{ element.text }}</a>
            </li>
          </ul>
        </nav>

        <div class="btn-wrapper">
          <a href="#" class="btn">Free quote</a>
        </div>
        </div>
      </div>


  </header>
</template>

<script>
import SocialLinks from "./SocialLinks.vue";

export default {
  name: 'AppHeadeader',
  components: {
    SocialLinks,
  },
  data(){
    return{
      activeElement: 0,
      navElements: [
        {
          text: 'Home',
          url: '#'
        },
        {
          text: 'Rates',
          url: '#'
        },
        {
          text: 'Testimonials',
          url: '#'
        },
        {
          text: 'FAQ',
          url: '#'
        },
        {
          text: 'Blog',
          url: '#'
        },
        {
          text: 'Contact',
          url: '#'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

header{
  width: 100%;
  
    
    .cta{
      background-color: $brand-primary-color;
      height: $app-header-cta-height;

      .container{
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .call-section{
          color: white;
          font-size: .8rem;
          
          i{
            margin-right: 5px;
          }
      }
    }
  }

  .navbar{
    height: $app-header-navbar-height;

    .container{
      height: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;

      .logo-wrapper{
        height: 60%;

        img{
          height: 100%;
          width: auto;
        }
      }

      nav{
        
        ul{

          li{

            margin: 0 10px;

            a{
              padding: 5px;
              text-decoration: none;
              text-transform: capitalize;
              color: black;
              font-size: .9rem;
              font-weight: 600;

              &.active{
                color: $brand-primary-color;
              }
            }
          }
        }
      }

    }

  }

}

</style>