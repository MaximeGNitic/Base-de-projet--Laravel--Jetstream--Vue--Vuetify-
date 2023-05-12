<script setup lang="ts">
import TextContent from './TextContent.vue';
const test = true;
</script>

<template>
<v-container>
  <v-card class="my-card">
    <v-card-title class="col-md-4 col-12">
      <slot name="image"></slot>
    </v-card-title>
    <v-card-text class="col-md-8 col-12">
      <v-card-title class="title">
        <slot name="title"></slot>
      </v-card-title>
      <TextContent>
        <template v-slot:listContent>
          <slot name="list"></slot>
        </template>
      </TextContent>
      <div class="col flex flex-center pt-6">
        <slot name="button"></slot>
      </div>
    </v-card-text>
    </v-card>
  </v-container>
</template>

<style scoped>
.my-card{
  width: 100%;
  background-color: #1E1E1E;
  border: 1px solid white;
    border-radius: 16px;
}
</style>