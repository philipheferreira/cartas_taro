<template>
  <q-page class="flex flex-center">
    <div class="q-pa-md q-gutter-sm">
      <q-btn color="red-5" @click="refresh">Mudar imagem</q-btn>

      <q-img :src="url" spinner-color="white" style="height: 140px; max-width: 150px" />
    </div>
  </q-page>
</template>

<script>
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  setup() {
    const url = ref('https://picsum.photos/500/300')

    return {
      url,
      refresh() {
        url.value = 'https://picsum.photos/500/300?t=' + Math.random()
      }
    }
  }
})
</script>
