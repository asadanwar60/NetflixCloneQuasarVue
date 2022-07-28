<template>
  <div class="gt-xs col-3">
    <q-list dense>
      <q-item>
        <q-item-section> {{ fTitle }}</q-item-section>
      </q-item>
    </q-list>
  </div>
  <div class="lt-sm col-6">
    <q-list dense>
      <q-item>
        <q-item-section> {{ fTitle }}</q-item-section>
      </q-item>
    </q-list>
  </div>
</template>

<script>
export default {
  props: { fTitle: String },
};
</script>

<style>
</style>
