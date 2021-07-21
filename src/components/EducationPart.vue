<template>
  <div class="row background educationBackground-desktop" :class="`${$q.screen.md  ? 'education-background_heightmd': ''}${$q.screen.sm ? 'education-background_heightsm educationBackground-mobile': ''}${$q.screen.xs ? 'education-background_heightxs educationBackground-mobile': ''} ${$q.screen.lg ? 'education-background_heightlg ': ''} ${$q.screen.xl ? 'education-background_heightxl': ''}`">
    <div class="col-12 q-mx-auto">
      <div class="row">
        <div class="col-xl-8 col-lg-8 col-md-8 col-sm-10 col-xs-10 q-mx-auto marginTop" >
          <h5 :class="`${$q.screen.xl  ? 'text-h4': ''}`" class="text-bold title_purple q-mt-lg q-mb-md" >My Education</h5>
          <p class="text-body1 text-justify">{{education}}</p>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
  export default {
    name: "Education",
    props:{
      education:String,
    }
  }
</script>
