<template>
  <img
    alt="banner"
    src="banner.png"
    width="100%"
    class="relative sm-hide xs-hide"
    :class="` ${$q.screen.md  ? 'heightmd': ''} ${$q.screen.lg ? 'heightlg': ''} ${$q.screen.xl ? 'heightxl': ''}`"
  />
</template>



<script>
  export default {
    name: "DesktopBanner",

  }
</script>

