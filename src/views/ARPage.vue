<template>
  <ion-page>

  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage} from '@ionic/vue';
import { CapacitorARKit } from 'capacitor-arkit';

export default defineComponent({
  name: 'ARPage',
  components: {
    IonPage
  },
  ionViewDidEnter() {
    CapacitorARKit.echo({'value': "test"});
  }
});
</script>

<style scoped>

</style>
