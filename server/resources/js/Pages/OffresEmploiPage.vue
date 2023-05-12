<script setup>
  import {useOffreStore} from '../stores/offresEmploi';
  const offreStore = useOffreStore();
  offreStore.getOffresEmploi(); 
  console.log(offreStore.listEmploi);
</script>

<template>
  <div>
    <h4 class="text-blue-grey-2 text-center">Offres d'emploi disponible</h4>
    <router-link class="flex justify-end text-8xl" to="/offresemploi/ajout"><q-btn color="secondary" text-color="black">Add</q-btn></router-link>
    <q-markup-table>
      <thead>
        <tr>
          <th class="text-center">Id</th>
          <th class="text-center">Experience(Annee)</th>
          <th class="text-center">Date publication</th>
          <th class="text-center">Debut mandat</th>
          <th class="text-center">Horaire</th>
          <th class="text-center">Langue</th>
          <th class="text-center">Info supplementaire</th>
          <th class="text-center">Actions</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="offre in offreStore.listEmploi" :key="offre.id">
          <td class="text-center">{{offre.id}}</td>
          <td class="text-center">{{offre.offre_nombreAnnee}}</td>
          <td class="text-center">{{offre.offre_datePublication}}</td>
          <td class="text-center">{{offre.offre_debutMandat}}</td>
          <td class="text-center">{{offre.offre_horaire}}</td>
          <td class="text-center">{{offre.offre_langue}}</td>
          <td class="text-center">{{offre.offre_infoSup}}</td>
          <td class="text-center"><router-link to="/offresemploi/modif">Modif</router-link></td>
          <!-- ici sa genre /offresemploi/modif/:id pour aller sur la page de modification avec l'id de l'offre -->
        </tr>
      </tbody>
    </q-markup-table>
  </div>
</template>