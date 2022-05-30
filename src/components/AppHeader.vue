<template>
  <header>
    <div class="container">

      <div class="cta">
        <div class="call-section">
          <i class="fas fa-phone-alt"></i>
          Call us for a Free Quote 1.800.555.6789
        </div>

        <SocialLinks/>
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
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

header{
  background-color: $brand-primary-color;
  width: 100%;
  
  .container{

    .cta{
      height: $app-header-cta-height;
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

}

</style>