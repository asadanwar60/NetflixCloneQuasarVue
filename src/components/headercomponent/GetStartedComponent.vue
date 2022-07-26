<!-- <template>
  <div class="text-center text-h6 q-mt-lg q-mb-sm">
    Ready to watch? Enter your email to create or restart your membership.
  </div>
</template>
<script>
export default {
  name: "GetStartedComponent",
};
</script> -->

<template>
  <div class="text-center text-h6 gt-sm q-pb-sm">
    Ready to watch? Enter your email to create or restart your membership.
  </div>
  <p class="text-center lt-md q-pa-none q-ma-none">
    Ready to watch? Enter your email to create or restart your membership.
  </p>
  <div class="row">
    <div class="col-9">
      <q-input
        type="email"
        bg-color="white"
        label-color="grey"
        color="grey"
        square
        standout
        bottom-slots
        v-model="text"
        label="Email address"
        counter
      >
      </q-input>
    </div>
    <div class="col-3">
      <q-btn color="red" size="lg" class="q-pt-md q-pb-sm" no-caps
        >Get Started</q-btn
      >
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

