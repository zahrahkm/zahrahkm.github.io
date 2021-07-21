<template>
  <div>
  <DesktopBanner></DesktopBanner>
  <MobileBanner></MobileBanner>
  <div class="row absolute-top justify-center ">
    <div class="col-md-10 col-lg-8 col-xl-6">
      <div class=" row justify-center content-stretch marginTop " style="height: 150px" >
        <div class="col-md-6 col-sm-10 col-xs-11">
          <div :class="$q.screen.lt.md ? 'text-center '   : 'text-left marginTop'" >
            <div :class=" ` ${$q.screen.sm  ? 'text-h3': ''} ${$q.screen.md ? 'text-h3': ''} ${$q.screen.xs ? 'text-h4': 'text-h2'}`">
              Hi,<br /> I'm Zahra Hakimi<br />
            </div>
            <p class=" justify-left  text-h6">
              {{bannerText}}
            </p>
            <Button :button="button"></Button>

          </div>
        </div>
        <div class=" col-md-6 col-sm-8 col-xs-9" :class="$q.screen.lt.md ? 'order-first'  : 'order-last'">
          <img
            src="/zahra.png"
            width="100%"
            alt=""
          />
        </div>
      </div>
    </div>
  </div>
  </div>
</template>
<script>
  import DesktopBanner from "components/DesktopBanner";
  import MobileBanner from "components/MobileBanner";
  import Button from "components/Button";
  export default {
    name:'Banner',
    components: {Button, MobileBanner, DesktopBanner},
    props:{
      bannerText:String
    },
    data(){
      return{
        button:[
          {name:'My CV',color:'light_purple',link:'#'},
          {name:'Contact',color:'light_blue',link:'#contact'}
        ]
      }
    }
  }
</script>
