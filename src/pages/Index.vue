<template>
  <q-page class="flex flex-center">
    <q-img src="../image/back_card.jpg" style="height: 450px; width: 300px;" label="Flip Menu">
      <q-menu transition-show="flip-right" transition-hide="flip-left">
        <q-list style="min-width: 100px">
          <q-item clickable>
            <q-item-section>Having fun</q-item-section>
          </q-item>
          <q-item clickable>
            <q-item-section>Crazy for transitions</q-item-section>
          </q-item>
          <q-separator />
          <q-item clickable>
            <q-item-section>Mind blown</q-item-section>
          </q-item>
        </q-list>
      </q-menu>
    </q-img>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'PageIndex',
});
</script>
