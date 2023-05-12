<script setup>
  import {onMounted } from 'vue';
//   import {useOffreStore} from 'stores/offresEmploi';


//   const offreStore = useOffreStore();


//   //Login
//   function ajoutOffresEmploiForm() {
//       offreStore.addOffreEmploi(experience.value, datePublication.value, debutMandat.value, horaire.value, langue.value, infoSup.value);
//   }

// onMounted(async () => {
//   await offreStore.getOffreEmploi(); 
//   console.log(offreStore.listEmploi);
// });
</script>

<template>
  <div>
    <h4 class="text-blue-grey-2 text-center">Modifier un offre d'emploi</h4>
    <form @submit.prevent="ajoutOffresEmploiForm">
      <input type="text" id="test">
      <q-input class="bg-blue-grey-2" v-model="offreStore.listEmploi.offre_nombreAnnee"  />
      <q-date class="bg-blue-grey-2" v-model="offreStore.listEmploi.offre_datePublication"/>
      <q-date class="bg-blue-grey-2" v-model="offreStore.listEmploi.offre_dateMandat"/>
      <q-input class="bg-blue-grey-2" label="Horaire" v-model="offreStore.listEmploi.offre_horaire"/>
      <q-input class="bg-blue-grey-2" label="Langue" v-model="offreStore.listEmploi.offre_langue"/>
      <q-input class="bg-blue-grey-2" label="Info Supplementaire" v-model="offreStore.listEmploi.offre_infoSup"/>

      <q-btn class="bg-blue-grey-2" label="Submit" type="submit"/>
    </form>
  </div>
</template>