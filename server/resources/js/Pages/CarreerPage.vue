<script setup lang="ts">
import TitleComponent from '../Components/TitleComponent.vue';
import CarrerApp from '../Components/CarrerApp.vue';
</script>

<template>
    <TitleComponent>
      <template v-slot:upTitle>
        Faire carrière
      </template>
      <template v-slot:underTitle>
        À la recherche d’un emploi ? Nous sommes votre tremplin vers différents employeurs du secteur industriel.
      </template>
    </TitleComponent>
    <div class="q-py-xl"></div>
    <div class="q-py-xl"></div>
    <div class="q-py-xl"></div>
    <div>
        <CarrerApp />  
    </div>
    <div class="q-py-xl"></div>
</template>