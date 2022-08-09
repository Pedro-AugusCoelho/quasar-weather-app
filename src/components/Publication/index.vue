<template>
    <q-card class="my-card q-pa-sm bg-grey-11" >
        <q-item clickable v-ripple  @click='openModal'>
          <q-item-section avatar>
            <q-icon color="primary" name="description" />
          </q-item-section>
          <q-item-section style="font-size:18px ; font-weight:500">No que você está pensando?</q-item-section>
        </q-item>
        <q-card-actions class="flex justify-between q-pa-none">
          <q-btn flat color="green-9" icon="videocam" label="Videos ao vivo" @click='openModal' />
          <q-btn flat color="cyan-14" icon="image" label="Foto/Vídeo" @click='openModal' />
          <q-btn flat color="deep-orange-13" icon="emoji_emotions" label="Sentimento/Atividade" @click='openModal' />
        </q-card-actions>
      </q-card>
</template>

<script>

export default {
  name: 'Publication',
  props: ['openModal']
}
</script>
