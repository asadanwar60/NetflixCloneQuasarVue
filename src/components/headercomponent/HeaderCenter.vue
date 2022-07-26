<template>
  <div class="absolute-full row justify-center items-center">
    <div class="col-md-6 col-sm-12 z-top">
      <div class="text-center text-h3 gt-sm text-bold q-mb-sm">
        Unlimited movies, TV shows and more.
      </div>
      <div class="text-center text-bold lt-md q-pa-none q-ma-none">
        Unlimited movies, TV shows and more.
      </div>
      <div class="text-center gt-sm text-h5 q-mb-md">
        Watch anywhere. Cancel anytime.
      </div>
      <p class="text-center lt-md q-pa-none q-ma-none">
        Watch anywhere. Cancel anytime.
      </p>
      <GetStartedComponent />
    </div>
  </div>
</template>
<script>
import GetStartedComponent from "./GetStartedComponent.vue";
export default {
  components: {
    GetStartedComponent,
  },
};
</script>
