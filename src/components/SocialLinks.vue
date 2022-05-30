<template>
  <div class="socials">
    <ul class="line-list">
      <li v-for="(element, index) in socialLinks" :key="index">
        <a :href="element.url" :title="element.social">
          <i :class="element.iconClass"></i>
        </a>
      </li>
    </ul>

    <!-- <i class="fab fa-facebook-f"></i>
    <i class="fab fa-twitter"></i>
    <i class="fab fa-instagram"></i>
    <i class="fab fa-youtube"></i> -->
  </div>
</template>

<script>
export default {
  name: 'SocialLinks',
  data(){
    return{
      socialLinks: [
        {
          social: 'facebook',
          iconClass: 'fab fa-facebook-f',
          url: '#',
        },
        {
          social: 'twitter',
          iconClass: 'fab fa-twitter',
          url: '#',
        },
        {
          social: 'instagram',
          iconClass: 'fab fa-instagram',
          url: '#',
        },
        {
          social: 'youtube',
          iconClass: 'fab fa-youtube',
          url: '#',
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.socials{
  color: $text-primary-color;
  background-color: transparent;

  ul{
    font-size: .8rem;

    li{
      margin: 0 5px;
      
      a{
        color: $text-primary-color;
      }
    }
  }
}

</style>