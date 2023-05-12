<template>
<div class="d-flex justify-center">
  <div class="d-flex flex-column text-white" style="width: 75%;">
    <div class="d-flex flex-column justify-center align-center text-center">
      <h2 class="text-h4-md">
        Pourquoi le projet est né ?
      </h2>
    </div>
    <div class="py-10"></div>
    <div class="d-flex flex-wrap justify-center align-center">
      <v-card class="d-flex flex-col mx-4 mb-8 box-item-1" max-width="350">
        <div class="text-2xl d-flex justify-start align-start">
            2006
        </div>
        <div>
            Démarrage d'un programme de formation avec le CFPBJ.    
        </div>
      </v-card>
      <v-card class="d-flex flex-col mx-4 mb-8 box-item" max-width="350" color="#D9D9D9">
          <div class="text-2xl ml-6">
            2017
          </div>
          <div class="ml-9">
            Démarrage cohorte crie. Diplôme reconnue par le ministère de l'éducation.
          </div>
      </v-card>
      <v-card class="d-flex flex-col mx-4 mb-8 box-item" max-width="350" color="#B2B2B2">
          <div class="text-2xl ml-6">
            2022
          </div>
          <div class="ml-8">
            Lancement de la première cohorte de formation sur mesure du programme Découverte
          </div>
      </v-card>
    </div>
  </div>
</div>
</template>


<style scoped>
.box-item-1 {
    height: 100px;
    -webkit-clip-path: polygon(91% 0, 100% 50%, 90% 100%, 0% 100%, 0 50%, 0% 0%);
    clip-path: polygon(91% 0, 100% 50%, 90% 100%, 0% 100%, 0 51%, 0% 0%);
}
.box-item {
    height: 100px;
    -webkit-clip-path: polygon(91% 0, 100% 50%, 90% 100%, 0% 100%, 10% 50%, 0% 0%);
    clip-path: polygon(91% 0, 100% 50%, 90% 100%, 0% 100%, 10% 50%, 0% 0%);
}

@media screen and (max-width: 1024px) {
    .mobile{
        flex-direction: column;
    }
    .box-item-1 {
        height: 100px;
        padding: 5px 10px;
        text-align: center;
        -webkit-clip-path: polygon(100% 0, 100% 85%, 50% 100%, 0 85%, 0 0, 50% 0);
        clip-path: polygon(100% 0, 100% 85%, 50% 100%, 0 85%, 0 0, 50% 0);
    }
    .box-item {

        height: 100px;
        padding: 5px 10px;
        text-align: center;
        -webkit-clip-path: polygon(100% 0, 100% 85%, 50% 100%, 0 85%, 0 0, 50% 8%);
        clip-path: polygon(100% 0, 100% 85%, 50% 100%, 0 85%, 0 0, 50% 8%);
    }
}
</style>