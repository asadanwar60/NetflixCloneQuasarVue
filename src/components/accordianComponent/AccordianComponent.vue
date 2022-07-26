 <template>
  <q-list bordered>
    <q-expansion-item
      group="somegroup"
      :label="label"
      header-class="bg-grey text-white border-white text-h5 q-pt-lg q-pb-lg q-pl-lg q-pr-lg"
    >
      <q-separator />
      <q-card>
        <q-card-section class="bg-grey text-white text-h6">
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
