 <template>
  <q-list bordered class="gt-xs">
    <q-expansion-item
      group="somegroup"
      :label="label"
      header-class="bg-grey text-white border-white text-h5 q-pt-lg q-pb-lg q-pl-lg q-pr-lg"
    >
      <div>{{ label }}</div>
      <q-separator />
      <q-card>
        <q-card-section class="bg-grey text-white text-h6">
          {{ description }}
        </q-card-section>
      </q-card>
    </q-expansion-item>
  </q-list>
  <q-list bordered class="lt-sm">
    <q-expansion-item
      group="somegroup"
      :label="label"
      header-class="bg-grey text-white border-white text-h6 "
    >
      <div>{{ label }}</div>
      <q-separator />
      <q-card>
        <q-card-section class="bg-grey text-white">
          {{ description }}
        </q-card-section>
      </q-card>
    </q-expansion-item>
  </q-list>
</template>
<script>
export default {
  props: { label: String, description: String },
};
</script>
