<template>
  <ul class="relative-position row text-subtitle1">
    <a :href="item.link" v-for="item in menu" :key="item.name" style="text-decoration: none;list-style: none" >
       <li  class="q-mx-lg q-mt-xs text-grey-9 ">
         {{ item.name }}
      </li>
    </a>
  </ul>
</template>


<script>
  export default {
    name: "MenuItems",
    props:{
      menu:Array,
    }
  }
</script>
