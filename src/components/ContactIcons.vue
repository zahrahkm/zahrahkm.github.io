<template>
    <social-icon :socialIcon="socialIcons" >
    </social-icon>
</template>

<script>
  import SocialIcon from "components/SocialIcon";
  export default {
    name: "ContactIcons",
    components: { SocialIcon }
    ,data(){
      return{
        socialIcons:[
         {name:'fab fa-github' , link:'https://github.com/zahrahkm' }
        ,{name:'fab fa-linkedin', link:'https://www.linkedin.com/in/zahra-hakimi-5972a0b2/' }
        ,{name:'fab fa-stack-overflow', link:'https://stackoverflow.com/users/14908293/zahra-hakimi' }
        ,{name:'fab fa-instagram-square', link:'https://www.instagram.com/zahra.hakimii/' }
        ],
      }
    }
  }
</script>
