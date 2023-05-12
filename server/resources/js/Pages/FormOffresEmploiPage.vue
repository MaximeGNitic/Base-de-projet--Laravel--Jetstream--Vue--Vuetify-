<script setup>
    // import {useOffreStore} from 'stores/offresEmploi';
    // import { ref } from 'vue'

    // const offreStore = useOffreStore();

    // const experience = ref(null);
    // const datePublication = ref(null);
    // const debutMandat = ref(null);
    // const horaire = ref(null);
    // const langue = ref(null);
    // const infoSup = ref(null);

    // //Login
    // function ajoutOffresEmploiForm() {
    //     offreStore.addOffreEmploi(experience.value, datePublication.value, debutMandat.value, horaire.value, langue.value, infoSup.value);
    //     console.log(experience.value);
    // }
</script>

<template>
  <div>
    <h4 class="text-blue-grey-2 text-center">Ajouter un offre d'emploi</h4>
    <form @submit="ajoutOffresEmploiForm">
        <q-input class="bg-blue-grey-2" label="Experience(Annee)" v-model="experience"/>
        <q-date class="bg-blue-grey-2" v-model="datePublication"/>
        <q-date class="bg-blue-grey-2" v-model="debutMandat"/>
        <q-input class="bg-blue-grey-2" label="Horaire" v-model="horaire"/>
        <q-input class="bg-blue-grey-2" label="Langue" v-model="langue"/>
        <q-input class="bg-blue-grey-2" label="Info Supplementaire" v-model="infoSup"/>

        <q-btn class="bg-blue-grey-2" label="Submit" type="submit"/>
    </form>
  </div>
</template>