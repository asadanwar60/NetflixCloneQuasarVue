<template>
  <q-separator color="grey" size="6px" />
  <div :class="id % 2 == 0 ? 'row' : 'row reverse'" class="justify-center">
    <div class="gt-sm col-5 q-pa-xl">
      <q-img :src="`src/assets/images/${image}`"></q-img>
    </div>
    <div class="gt-sm col-5 q-pt-xl q-pr-xl q-pb-xl q-mt-xl">
      <div class="text-h3 text-white text-bold q-mt-xl q-pb-md">
        {{ heading }}
      </div>
      <div class="text-h5 text-white">
        {{ subHeading }}
      </div>
    </div>

    <div class="q-pa-lg">
      <div class="lt-md col-12 q-mt-lg">
        <div class="text-h5 text-white text-bold text-center">
          {{ heading }}
        </div>
        <p class="text-white text-center q-pt-md">
          {{ subHeading }}
        </p>
      </div>
      <div class="lt-md col-12 q-mb-lg q-pa-none">
        <q-img :src="`src/assets/images/${image}`"></q-img>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    id: Number,
    subHeading: String,
    heading: String,
    image: String,
  },
  name: "MidSectionComponent",
};
</script>

<style>
</style>
