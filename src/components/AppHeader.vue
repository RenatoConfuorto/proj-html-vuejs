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

    <div class="motto">
      <div class="container-small">
        <h3>Moving without the hassle</h3>
        <h1>We make it simple</h1>
        <h3>professional service with quality and customer satisfaction</h3>
      </div>
    </div>

    <div class="free-quote">
      <i class="fas fa-paper-plane"></i> Get a free quote online now!
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
  height: 70vh;
  background-image: url(../assets/img/avada-movers-homeherobackground-final.jpg);
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
    
    .cta{
      background-color: $brand-primary-color;
      height: $app-header-cta-height;

      .container{
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .call-section{
          color: $text-primary-color;
          font-size: .8rem;
          
          i{
            margin-right: 5px;
          }
      }
    }
  }

  .navbar{
    height: $app-header-navbar-height;
    background-color: transparent;

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
              color: $text-secondary-color-dark;
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

  .motto{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-grow: 1;

    .container-small{
      text-align: center;
      text-transform: uppercase;

      h3{
        font-size: .8rem;
        color: $text-secondary-color;
        margin-bottom: 10px;
      }

      h1{
        font-size: 2.5rem;
        color: $text-secondary-color-dark;
        margin-bottom: 10px;
      }
    }
  }

  .free-quote{
    height: 4rem;
    background-color: $brand-secondary-color;
    color: $text-primary-color;
    text-align: center;
    text-transform: uppercase;
    font-size: .8rem;
    line-height: 4rem;
  }

}

</style>