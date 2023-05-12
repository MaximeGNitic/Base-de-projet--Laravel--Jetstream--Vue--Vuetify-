<script setup lang="ts">
import TextContent from './TextContent.vue';
</script>

<template>
  <v-container class="my-card">
    <v-row class="align-center justify-center">
      <v-col cols="12" md="4">
        <slot name="image"></slot>
      </v-col>
      <v-col cols="12" md="8">
        <v-row>
          <v-col cols="12">
            <slot class="title" name="title"></slot>
          </v-col>
          <v-col cols="12">
            <v-card-text>
              <template v-slot:default>
                <slot name="text"></slot>
              </template>
            </v-card-text>
          </v-col>
          <v-col cols="12" class="d-flex justify-end pt-5">
            <slot name="button"></slot>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
  <v-container class="q-py-xl">
    <v-row justify="center">
      <v-col cols="12" md="8">
        <v-card class="my-card">
          <v-row>
            <v-col cols="4" class="self-center">
              <slot name="image"></slot>
            </v-col>
            <v-col cols="8" class="flex-center">
              <div class="title">
                <slot name="title"></slot>
              </div>
              <TextContent class="flex flex-start">
                <template v-slot:underTitle>
                  <slot name="text"></slot>
                </template>
              </TextContent>
              <div class="col flex flex-start q-pt-lg">
                <slot name="button"></slot>
              </div>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
    <v-row justify="center">
      <v-col cols="12" md="8">
        <v-card class="my-card">
          <v-row>
            <v-col cols="8" class="flex-center">
              <div class="title">
                <slot name="title2"></slot>
              </div>
              <TextContent class="flex flex-start">
                <template v-slot:underTitle>
                  <slot name="text2"></slot>
                </template>
              </TextContent>
              <div class="col flex flex-start q-pt-lg">
                <slot name="button2"></slot>
              </div>
            </v-col>
            <v-col cols="4" class="self-center">
              <slot name="image2"></slot>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
.my-card{
  width: 100%;
  min-width:300px;
  background-color: #1E1E1E;
  border: 1px solid white;
}
</style>