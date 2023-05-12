<script setup>
import card from '../assets/card.png';
</script>

<template>
  <v-container>
    <v-row justify-center>
      <v-col cols="12" md="4">
        <v-card class="my-card" flat>
          <v-img :src="card"></v-img>
          <v-card-title class="text-h4">
            <slot name="Title"></slot>
          </v-card-title>
          <v-card-text class="q-py-md">
            <slot name="Description"></slot>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
.my-card{
    min-width: 350px;
    max-width: 425px;
    border-radius: 16px;
    background: transparent;
}
</style>