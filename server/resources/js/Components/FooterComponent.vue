<script setup>
import { ref, computed } from 'vue'
import logo2 from '../assets/logo2.png'
const mobile = ref(window.innerWidth < 600)
window.addEventListener('resize', () => {
  mobile.value = window.innerWidth < 600
})





</script>
<template>
  <div v-if="mobile" style="min-height: 20vh;" class="text-center">
        <div class="flex-row justify-center">
        <q-img
          src="../assets/logo2.png"
          style="height: 75px; width: 75px"
          :style="{ transform: 'scale(2)' }"
        />
        </div>
        <div class="row flex justify-evenly">
          <div class="col-5">
              <div class="row">Acceuil</div>
              <div class="row">Nos services</div>
              <div class="row">Faire carrière</div>
              
          </div>
          <div class="col-5">
              <div class="row flex justify-end">Contactez-nous</div>
              <div class="row flex justify-end">Qui sommes-nous ?</div>
              <div class="row flex justify-end">Programme de formation</div>
          </div>
        </div>
  </div>
  <div v-else class="pa-8 text-center text-weight-light">
    <div class="d-flex justify-evenly" style="height: 200px">
      <v-col cols="2" class="d-flex justify-center align-center">
        <v-img :src="logo2" style="height: 75px; max-width: 75px" :style="{ transform: 'scale(2)' }" />
      </v-col>
      <v-col cols="2" class="d-flex flex-col justify-around">
        <div>Acceuil</div>
        <div>Nos services</div>
        <!-- <div>
          <v-btn color="white" text-color="black" class="q-px-xl">
            Se connecter
          </v-btn>
        </div> -->
        <div></div>
      </v-col>
      <v-col cols="2" class="d-flex flex-col justify-around">
        <div>Programme de formation découverte</div>
        <div>Faire carrière</div>
        <div></div>
      </v-col>
      <v-col cols="2" class="d-flex flex-col justify-around">
        <div>Contactez-nous</div>
        <div>Qui sommes-nous ?</div>
        <div>
          <v-icon size="2rem">mdi-facebook</v-icon>
        </div>
      </v-col>
    </div>
  </div>
</template>
