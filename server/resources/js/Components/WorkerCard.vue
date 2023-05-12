<script setup>
import card from '../assets/card.png';
</script>

<template>
<v-card class="my-card pa-8" flat>
  <v-img :src="card">
    <div class="absolute-bottom text-center text-h6">
      <slot name="cardTitle"></slot>
    </div>
  </v-img>
</v-card>
</template>

<style scoped>
.my-card{
    min-width: 225px;
    max-width: 225px; /*temp*/
    border-radius: 16px;
    background: transparent;
}
</style>