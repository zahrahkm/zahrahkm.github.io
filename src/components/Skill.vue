<template>
  <div class="row"  height="50%">
    <div class="col-10 q-mx-auto">
      <div class="row ">
        <div class="col-lg-4 col-md-4 col-12-sm col-12-xs q-my-xl q-mx-auto " style="margin-top: -50px;">
          <h5 :class="`${$q.screen.xl  ? 'text-h4': ''}`" class="text-bold title_purple" >My skills</h5>
          <div class="row">
            <div class="col-12" v-for="i in Skills" :key="i.title" >
              <div class="flex row justify-between q-mb-md">
                <p>{{i.skill}}</p>
                <p>{{i.percentage}}%</p>
                <q-linear-progress :value="i.percentage+'%'" rounded color="purple" style="height: 10px"/>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-md-4 col-12-sm col-12-xs q-mx-auto" >
          <q-img src="/skills.png"></q-img>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Skill",
    props:{
      Skills:Array,
    }
  }
</script>
