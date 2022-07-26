<template>
  <q-select
    style="border: 2px solid white"
    v-model="model"
    :options="options"
  />
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    return {
      model: ref("Google"),

      options: ["Google", "Facebook", "Twitter", "Apple", "Oracle"],
    };
  },
};
</script>


<!-- <template>
  <q-select
    square
    outlined
    class="text-white"
    v-model="model"
    :options="options"
    label="Square outlined"
  />
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    return {
      model: ref(null),
      options: ["Google", "Facebook", "Twitter", "Apple", "Oracle"],
    };
  },
};
</script> -->
