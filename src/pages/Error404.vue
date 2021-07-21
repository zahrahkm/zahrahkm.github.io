<template>
  <div class="notfound_background  fullscreen " >
    <div class="text-cyan-4 text-center q-pa-md flex flex-center">
      <div>
        <div style="font-size: 30vh">
          404
        </div>

        <div class="text-h2" style="opacity:.6">
          Oops. Nothing here...
        </div>

        <q-btn
          class="q-mt-xl q-px-md q-py-sm"
          color="purple-4"
          text-color="white"
          unelevated
          to="/"
          label="Go Home"
          no-caps
          rounded
        />
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: 'Error404'
}
</script>
<style>
  .notfound_background{
    background-image: url("/404.png");
    background-size: cover;
    width: 100%;
    align-items: center;
    justify-content: center;
    height: 100%;
  }
</style>
