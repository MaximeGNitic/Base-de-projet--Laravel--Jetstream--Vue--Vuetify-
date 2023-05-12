<script setup>
import { Link } from '@inertiajs/vue3';
import { ref, computed } from 'vue'
// import { useRouter } from 'vue-router'

// const router = useRouter()

const onMainDoeuvreClick = () => {
  console.log('onMainDoeuvreClick')
    Link.push('/main-doeuvre')
}

const onSoutienClick = () => {
  console.log('onSoutienClick')
    Link.push('/soutien')
}

const onFormationClick = () => {
  console.log('onFormationClick')
    Link.push('/formation')
}

</script>

<template>
<v-menu offset-y>
  <template v-slot:activator="{ on }">
    <v-btn v-on="on">
      <span>Nos services</span>
      <v-icon>mdi-menu-down</v-icon>
    </v-btn>
  </template>

  <v-list>
    <v-list-item @click="onMainDoeuvreClick">
      <v-list-item-title>Main d'oeuvre</v-list-item-title>
    </v-list-item>
    <v-list-item @click="onFormationClick">
      <v-list-item-title>Formation découverte</v-list-item-title>
    </v-list-item>
    <v-list-item @click="onSoutienClick">
      <v-list-item-title>Soutien usine</v-list-item-title>
    </v-list-item>
  </v-list>
</v-menu>
  </template>