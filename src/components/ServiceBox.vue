<template>
  <div class="row">
    <div class="col-10 q-mx-auto">
      <div class="row">
        <div class="col-lg-3 col-md-6 col-sm-6 col-xs-12 " v-for="i in ServiceBox" :key="i.title"  align="center">
          <q-img  :src="i.image" class="responsive" width="50" height="80"></q-img>
          <h5 :class="`${$q.screen.xl  ? 'text-h4': ''}`" class="q-mb-md" >{{i.title}}</h5>
          <p class="text-body1" style="width: 60%" >{{i.text}}</p>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
  export default {
    name: "SeviceBox",
    props:{
      ServiceBox:Array,
    }
  }
</script>
