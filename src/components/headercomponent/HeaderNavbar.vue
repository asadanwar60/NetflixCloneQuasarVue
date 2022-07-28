<template>
  <q-toolbar class="transparent z-top text-white">
    <q-toolbar-title class="gt-xs q-ml-lg">
      <img src="src/assets/images/logo.png" style="width: 130px"
    /></q-toolbar-title>
    <q-toolbar-title class="lt-sm">
      <img src="src/assets/images/logo.png" style="width: 80px"
    /></q-toolbar-title>
    <q-btn-dropdown label="English" no-caps outline class="gt-xs q-mr-lg">
      <q-list>
        <q-item>
          <q-item-section>Hindi</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>English</q-item-section>
        </q-item>
      </q-list>
    </q-btn-dropdown>
    <q-btn-dropdown label="English" no-caps outline size="sm" class="lt-sm">
      <q-list>
        <q-item>
          <q-item-section>Hindi</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>English</q-item-section>
        </q-item>
      </q-list></q-btn-dropdown
    >
    <q-btn label="English" no-caps color="red" class="q-mr-lg gt-xs" />
    <q-btn
      label="English"
      no-caps
      color="red"
      size="sm"
      class="q-ml-md lt-sm"
    />
  </q-toolbar>
</template>
