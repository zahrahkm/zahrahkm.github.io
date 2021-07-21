<template>
  <img
    alt="mobile banner"
    src="~assets/mobileBanner.png"
    width="100%"
    :class="` ${$q.screen.sm  ? 'heightsm': ''} ${$q.screen.xs  ? 'heightxs': ''} `"
    class="relative lg-hide xl-hide md-hide"
  />
</template>


<script>
  export default {
    name: "MobileBanner",

  }
</script>
