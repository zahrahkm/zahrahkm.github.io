<template>
  <div class="background aboutBackground-mobile" :class="` ${$q.screen.md  ? ' About-background_heightmd aboutBackground-desktop': ''} ${$q.screen.lg ? 'About-background_heightlg aboutBackground-desktop': ''} ${$q.screen.xl ? 'About-background_heightxl aboutBackground-desktop': ''}`">
    <div class="row q-mt-lg">
      <div class="col-xl-8 col-lg-8 col-md-8 col-sm-10 col-xs-10 q-mx-auto">
        <div class="row">
          <div class="col-12 text-dark q-mx-auto q-my-xl" v-for="i in AboutMe" :key="i.title" style="margin-top: 100px" >
            <h5 :class="`${$q.screen.xl  ? 'text-h4': ''}`" class="q-mb-md text-bold title_purple" >{{i.title}}</h5>
            <p class="text-body1 text-dark">{{i.text}}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>







<script>
  export default {
    name: "AboutMe",
    props:{
      AboutMe:Array

    }
  }
</script>



