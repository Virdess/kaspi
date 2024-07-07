<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-back-button />
        </ion-buttons>
        <ion-title>Удостоверение личности</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content>
      <ion-segment>
        <ion-segment-button value="document" checked>
          <ion-label>Документ</ion-label>
        </ion-segment-button>
        <ion-segment-button value="details">
          <ion-label>Реквизиты</ion-label>
        </ion-segment-button>
      </ion-segment>

      <div style="text-align: center; margin-top: 20px;">
        <!-- Здесь можно использовать <img> вместо <div> для реального изображения -->
        <div style="border: 1px solid black; display: inline-block; padding: 20px;">
          Изображение
        </div>
      </div>
    </ion-content>

    <ion-footer>
      <ion-grid>
        <ion-row>
          <ion-col size="12">
            <ion-button expand="block" color="primary">Предъявить документ</ion-button>
          </ion-col>
          <ion-col size="12">
            <ion-button expand="block" color="light">Отправить документ</ion-button>
          </ion-col>
        </ion-row>
      </ion-grid>
    </ion-footer>
  </ion-page>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'HomePage',
});
</script>
