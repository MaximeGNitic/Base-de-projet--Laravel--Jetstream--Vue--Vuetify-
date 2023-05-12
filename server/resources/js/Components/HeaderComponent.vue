<script setup>
import { ref } from 'vue'
import ServiceHeader from './ServiceHeader.vue';
import logo2 from '../assets/logo2.png'
const mobile = ref(window.innerWidth < 1020)
window.addEventListener('resize', () => {
  mobile.value = window.innerWidth < 1020
})
</script>

<template>
    <div v-if="mobile" class="q-pa-md text-center text-h5" style="height: 30vh;">

    <div class="row">
      <div class="col flex flex-start">
        <q-btn icon="menu" style="font-size: 1.25em">
        <q-menu
          transition-show="scale"
          transition-hide="scale"
        >
          <q-list style="min-width: 100px">
            <q-item clickable>

              <q-item-section>Nos services</q-item-section>
            </q-item>
            <q-item clickable>
              <q-item-section>Carrière</q-item-section>
            </q-item>
            <q-separator />
            <q-item clickable>
              <q-item-section>Qui sommes-nous ?</q-item-section>
            </q-item>
            <q-item clickable>
              <q-item-section>Nous joindre</q-item-section>
            </q-item>
            <q-item>
              <q-item-section>
                <ServiceHeader />
              </q-item-section>
            </q-item>
            <router-link to="/carriere" style="text-decoration: none; color: inherit;">
              <q-item clickable>
                <q-item-section>CARRIÈRE</q-item-section> 
              </q-item>
            </router-link>
            <q-separator />
            <router-link to="/minopro" style="text-decoration: none; color: inherit;">
              <q-item clickable>
                  <q-item-section>QUI SOMMES-NOUS ?</q-item-section>
              </q-item>
            </router-link>
            <router-link to="/contact" style="text-decoration: none; color: inherit;">
              <q-item clickable>
                  <q-item-section>NOUS JOINDRE</q-item-section>
              </q-item>
            </router-link>

          </q-list>
        </q-menu>
      </q-btn>
      </div>
      <div class="col flex justify-end">


        <router-link to="/" style="text-decoration: none; color: inherit;">

        <q-img
          src="../assets/logo2.png"
          style="height: 100px; width: 100px"
          :style="{ transform: 'scale(2)' }"
        />

        </router-link>

      </div>
    </div>
  </div>



  <div v-else class="pa-8 text-slate-700" max-height="30vh">
    <div class="py-3 px-6">
    <v-row class="d-flex justify-between align-center">
      <v-col cols="auto">
        <ServiceHeader class="link" />
      </v-col>
      <v-col cols="auto">
        <!-- <link class="link" to="/carriere" > -->
          CARRIÈRE
        <!-- </link> -->
      </v-col>
      <v-col cols="auto">
        <!-- <LINK to="/" style="text-decoration: none; color: inherit;"> -->
          <v-img
            :src="logo2"
            height="100"
            width="100"
            style="transform: scale(2)"
          />
        <!-- </LINK> -->
      </v-col>
      <v-col cols="auto">
        <!-- <router-link class="link" to="/minopro"> -->
          QUI SOMMES-NOUS ?
        <!-- </router-link> -->
      </v-col>
      <v-col cols="auto">
        <!-- <router-link class="link" to="/contact"> -->
          NOUS JOINDRE
        <!-- </router-link> -->
      </v-col>
    </v-row>
  </div>
  </div>
</template>

<style scoped>
.link {
  margin: 10px;
}
.link.active {
  color: #BF9266;
  text-decoration: none;
}
.link{
  color: white;
  text-decoration: none;
}
</style>

