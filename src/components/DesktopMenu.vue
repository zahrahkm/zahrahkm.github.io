<template>
  <div class="row">
    <q-img
      class="absolute-top  col-md-8 col-lg-6 col-xl-4 "
      src="/cloud.png" :class="` ${$q.screen.sm  ? 'hidden': 'show'} ${$q.screen.xs  ? 'hidden': 'show'}`">
      <Menu></Menu>
    </q-img>
  </div>
</template>



<script>
  import Menu from "components/Menu";
  export default {
    name: "DesktopMenu",
    components: {Menu},
    data(){
      return{
      }
    }
  }
</script>
