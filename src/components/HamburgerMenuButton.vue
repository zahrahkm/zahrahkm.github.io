<template>
  <!-- hamburger menu (button) -->
  <q-toolbar class=" absolute-top back q-mt-md q-ml-md  text-primary md-hide lg-hide xl-hide ">
    <q-fab
      color="purple"
      icon="menu"
      direction="up"
      @click="drawerLeftMethod"
    ></q-fab>
  </q-toolbar>
</template>

<script>

  export default {
    name:'HamburgeMenu',
    data(){
      return{

      }

    },
    methods:{
      drawerLeftMethod(){
        this.$emit('drawer')
      }
    }

  };
</script>
