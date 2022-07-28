<template>
  <div class="text-center text-h6 gt-sm q-pb-sm">
    Ready to watch? Enter your email to create or restart your membership.
  </div>
  <p class="text-center lt-md q-pa-none q-ma-none">
    Ready to watch? Enter your email to create or restart your membership.
  </p>
  <div class="gt-xs row">
    <div class="col-9 col-sm-8 col-md-8">
      <q-input
        type="email"
        maxlength="25"
        bg-color="white"
        label="Email address"
        label-color="grey"
        filled
        borderless
      >
      </q-input>
    </div>
    <div class="col-3 col-sm-4 col-md-4">
      <q-btn color="red" size="lg" no-caps>Get Started</q-btn>
    </div>
  </div>
  <div class="lt-sm row justify-center">
    <div class="col-12 q-mt-lg">
      <q-input
        type="email"
        maxlength="25"
        bg-color="white"
        label="Email address"
        label-color="grey"
        filled
        borderless
      >
      </q-input>
    </div>
    <div class="col-5 jus q-mt-md">
      <q-btn color="red" no-caps>Get Started</q-btn>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";

export default {
  name: "GetStartedComponent",
  setup() {
    return {
      text: ref(""),
    };
  },
};
</script>

