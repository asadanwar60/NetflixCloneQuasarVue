<template>
  <div class="absolute-full row justify-center items-center">
    <div class="gt-xs col-md-6 z-top">
      <div class="text-center text-h2 text-bold q-mt-xl q-mb-sm">
        Unlimited movies, TV shows and more.
      </div>

      <div class="text-center text-bold text-h5 q-mb-md">
        Watch anywhere. Cancel anytime.
      </div>
      <GetStartedComponent />
    </div>
    <div class="lt-sm col-xs-12 col-sm-12 z-top q-mt-xl">
      <div class="text-center text-h5 text-bold">
        Unlimited movies, TV shows and more.
      </div>
      <div class="text-center text-bold">Watch anywhere. Cancel anytime.</div>
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
