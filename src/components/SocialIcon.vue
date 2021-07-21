<template>
  <div>
    <a :href="i.link" v-for="i in socialIcon" :key="i.name" style="text-decoration: none" target="_blank">
       <q-icon :name="i.name"  size="md" color="light-blue-11" class="q-mx-xs socialIcon" />
    </a>
  </div>
</template>




<script>
  export default {
    name: "SocialIcon",
    props:{
    socialIcon:Array,

  }
  }
</script>



