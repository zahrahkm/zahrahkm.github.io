<template>
  <q-layout view="hHh lpR fFf">
    <q-header>
      <DesktopMenu></DesktopMenu>
      <HamburgeMenu v-on:drawer="drawerLeftChange"></HamburgeMenu>
    </q-header>
    <!-- hamburger menu  -->
    <q-drawer
      v-model="drawerLeft"
      :width="300"
      :breakpoint="100"
      elevated
      content-class=" text-dark"
    >
      <q-scroll-area class="fit">
        <div class="q-pa-sm q-mt-xl text-center" >
          <Menu class="column" ></Menu>
        </div>
      </q-scroll-area>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>




  </q-layout>
</template>

<script>
import MyFooter from "components/ContactIcons";
import HamburgeMenu from "components/HamburgerMenuButton";
import DesktopMenu from "components/DesktopMenu";
import Menu from "components/Menu";
export default {
  components: {Menu, DesktopMenu, HamburgeMenu },
  data() {
    return {
      drawerLeft: false
    };
  },methods:{
    drawerLeftChange(){
      this.drawerLeft=!this.drawerLeft
    }
  }
};
</script>
<style>

.q-drawer,
.q-drawer--left,
.q-drawer--standard {
  position: fixed;
}

</style>
