<script setup>
import Logocree from '../assets/LogoCree.png';
</script>

<template>
<div class="d-flex justify-center">
<v-card class="my-card" :style="{ borderRadius: '24px' }">
  <v-row no-gutters>
    <v-col cols="12" md="4" class="d-flex justify-center align-center">
      <v-img :src="Logocree" max-width="300" />
    </v-col>
    <v-col cols="12" md="8">
      <v-card-title class="text-white">
        <div class="title">
          <slot name="cardTitle"></slot>
        </div>
        <div class="under-title">
          <slot name="cardUnderTitle"></slot>
        </div>
        <div class="list-title">
          <slot name="listTitle"></slot>
        </div>
      </v-card-title>
      <v-card-text class="text-white">
        <div class="under-title">
          <slot name="listContent"></slot>
        </div>
      </v-card-text>
    </v-col>
  </v-row>
</v-card>
</div>
</template>

<style scoped>
.my-card{
  width: 100%;
  max-width: 75%;
  background-color: transparent;
  border: 1px solid white;
}

/* .title
    font-style: normal
    font-weight: 400
    font-size: 45px
    line-height: 55px
    text-transform: uppercase

.under-title
    font-style: normal
    font-weight: 400
    font-size: 16px
    line-height: 24px

.list-title
    font-style: normal
    font-weight: 400
    font-size: 24px
    line-height: 24px */
</style>