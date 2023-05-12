<script setup>
import HeaderComponent from '../Components/HeaderComponent.vue';
import FooterComponent from '../Components/FooterComponent.vue';
</script>

<template>
  <v-app>
    <HeaderComponent />

    <v-main>
      <v-container fluid>
        <slot />
      </v-container>
    </v-main>

    <FooterComponent />
  </v-app>
</template>