<template>
  <div class="q-pa-md q-gutter-sm" >
    <a :href="i.link" v-for="i in button" :key="i.name"  style="text-decoration: none;list-style: none" class=" text-grey-9 ">
      <q-btn :class="i.color"  rounded :label="i.name" padding="10px 50px"/>
    </a>
  </div>
</template>



<script>
  export default {
    name:'Button',
    props:{
      button:Array
    }
  }
</script>
