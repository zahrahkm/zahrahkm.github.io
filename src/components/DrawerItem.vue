<template>
  <q-drawer
    :width="300"
    :breakpoint="100"
    elevated
    content-class=" text-dark"
    :checked="checked"
    @change="$emit('change', $event.target.checked)"

  >
    <q-scroll-area class="fit">
      <div class="q-pa-sm q-mt-xl text-center">
        <div v-for="i in 100" :key="i">{{i}}</div>
      </div>
    </q-scroll-area>
  </q-drawer>
</template>


<script>

  export default {
   name:'DrawerItem',
    props:{
      checked:Boolean
   }
  };
</script>
