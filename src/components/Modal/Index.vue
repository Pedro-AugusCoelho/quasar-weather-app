<template>
    <q-dialog v-model="isShow" persistent>
      <q-card style="width: 700px; max-width: 80vw;">
        <q-card-section class="row items-center q-pb-none">
          <div class="text-h6 text-center">Criar uma publicação</div>
          <q-space />
          <q-btn icon="close" flat round dense v-close-popup @click="closed" />
        </q-card-section>

        <q-separator class="q-mt-sm" />

        <q-card-section style="max-height: 50vh" class="scroll q-px-sm" >
          <q-input filled  color="teal-5" v-model="text" label="No que você esta pensando" class='full-width' />
        </q-card-section>

        <q-card-actions>
          <q-btn label="Publicar" color="secondary" v-close-popup @click="closed" class="full-width" />
        </q-card-actions>
      </q-card>
    </q-dialog>
</template>

<script>

export default {
  name: 'Modal',
  props: ['show'],
  watch: {
    show () {
      this.isShow = this.show
    },
    isShow () {
    }
  },
  data () {
    return {
      isShow: false,
      text: ''
    }
  },
  methods: {
    closed () {
      this.$emit('closed', this.isShow)
    }
  }
}
</script>
