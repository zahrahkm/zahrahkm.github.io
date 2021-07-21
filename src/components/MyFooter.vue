<template>
  <div class="row background contactBackground">
    <div class="col-10 q-mx-auto">
      <div class="row justify-center ">
        <div class="col-xl-6 col-lg-6 col-md-6 col-sm-7 col-xs-12" >
          <h5 :class="`${$q.screen.xl  ? 'text-h4': ''}`" class="text-bold title_purple" >Contact with me</h5>
            <p class="text-body1 text-justify">
              If you have any suggestions, ideas, or related projects to work on, you can get in touch with me via connections mentioned below.
              <br>
            <span class="text-bold q-mt-lg">Email me at: </span>
              <br>zahrahakimi777@gmail.com
          </p>
          <ContactIcons class="q-mt-lg"></ContactIcons>
        </div>
        <div class="col-xl-4 col-lg-4 col-md-4 col-sm-5 col-xs-8">
          <q-img src="contact.png" ></q-img>
        </div>
      </div>
    </div>
  </div>
</template>



<script>

  import ContactIcons from "components/ContactIcons";
  export default {
    name: "MyFooter",
    components: {ContactIcons},
    data(){
      return {
      }
    }
  }
</script>
