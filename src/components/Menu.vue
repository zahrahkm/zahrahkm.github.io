<template>
      <MenuItems :menu="menu" ></MenuItems>
</template>



<script>
  import MenuItems from "components/MenuItems";
  export default {
    name: "Menu",
    components: {MenuItems},
    data(){
      return{
        menu: [
          {name:"Home" , link:"#"},
          {name:"Skills" , link:"#skill"},
          {name:"Experience" , link:"#experience"},
          {name:"contact" , link:"#contact"},
        ]
      }
    }
  }
</script>
