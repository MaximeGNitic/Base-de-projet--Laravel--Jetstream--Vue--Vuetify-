<script setup>
import CardLogo from '../Components/CardLogo.vue';
import CarrerApp from '../Components/CarrerApp.vue';
import HomeCard from '../Components/HomeCard.vue';
import OurTeam from '../Components/OurTeam.vue';
import ProcessCard from '../Components/ProcessCard.vue';
import WhyProject from '../Components/WhyProject.vue';
import WorkerCard from '../Components/WorkerCard.vue';
import WorkerCard2Vue from '../Components/WorkerCard2.vue'; 
import WorkListCard from '../Components/WorkListCard.vue';
</script>

<template>
  <div>
    <h1>Ceci est HomePage</h1>
    <v-btn>
      Test
    </v-btn>
    <CardLogo/>
    <div class="py-16"></div>
    <CarrerApp/>
    <div class="py-16"></div>
    <HomeCard/>
    <div class="py-16"></div>
    <OurTeam/>
    <div class="py-16"></div>
    <ProcessCard/>
    <div class="py-16"></div>
    <WhyProject/>
    <div class="py-16"></div>
    <WorkerCard/>
    <div class="py-16"></div>
    <WorkerCard2Vue/>
    <div class="py-16"></div>
    <WorkListCard/>


  </div>
</template>

<!-- <script setup lang="ts">

// import TopHome from 'src/components/HomeComponent/TopHome.vue';
import TitleComponent from 'src/components/TitleComponent.vue';
import ButtonPrimary from 'src/components/ButtonPrimary.vue';
import WorkerCard from 'src/components/WorkerCard.vue';
import HomeCard from 'src/components/HomeCard.vue';
</script> -->

<!-- <template>
  <TitleComponent>
      <template v-slot:upTitle>
        L’endroit parfait pour trouver des employés miniers
      </template>
      <template v-slot:underTitle>
        Nous sommes une agence de placement spécialisée dans le domaine minier. Nous offrons des services de recrutement et de placement de personnel pour les entreprises minières.
      </template>
  </TitleComponent>
  <div class="q-py-xl"></div>
  <div class="flex flex-center">
    <ButtonPrimary label="Trouver un employé" />
  </div>
  <div class="q-py-xl"></div>
  <div class="q-py-xl"></div>

  <div class="flex flex-center">
    <div class="row flex-center" style="width: 75%;">
      <WorkerCard class="col-4">
        <template v-slot:cardTitle>
          Service de main-s’oeuvre qualifiée
        </template>
      </WorkerCard>
      <WorkerCard class="col-4">
        <template v-slot:cardTitle>
          Programme de formation découverte
        </template>
      </WorkerCard>
      <WorkerCard class="col-4">
        <template v-slot:cardTitle>
          Soutien en usine
        </template>
      </WorkerCard>
    </div>
  </div>

  <div class="q-py-xl"></div>
  <div class="q-py-xl"></div>
  <HomeCard>
    <template v-slot:image>
      <q-img src="../assets/card2.png" />
    </template>
    <template v-slot:title>
      <div class="title">
        Faire carrière chez minopro
      </div>
    </template>
    <template v-slot:text>
      <div class="flex flex-start">
        Lorem ipsum dolor sit amet consectetur. Varius euismod et arcu habitasse mauris id non augue metus.
        Molestie felis auctor nibh fringilla. Est tincidunt faucibus aliquet in felis integer egestas.
        Feugiat amet mattis vel consequat suspendisse vehicula. Dui egestas arcu morbi ultrices egestas pharetra. Netus auctor gravida netus tempus varius pretium.
        Feugiat amet mattis vel consequat suspendisse vehicula. Dui egestas arcu morbi ultrices egestas pharetra. Netus auctor gravida netus tempus varius pretium.
      </div>
    </template>
    <template v-slot:button>
      <q-btn
        color="primary"
        label="En savoir plus"
        class="q-mt-md"
      />
    </template>
    <template v-slot:title2>
      <div class="title">
        Qui sommes-nous
      </div>
    </template>
    <template v-slot:text2>
      <div class="flex flex-start">
        <div>
          Lorem ipsum dolor sit amet consectetur. Ornare id amet pellentesque at vitae metus amet. Placerat facilisis ac faucibus vitae nulla in augue nullam neque.
        </div>
        <div>
          Lorem ipsum dolor sit amet consectetur. Ornare id amet pellentesque at vitae metus amet. Placerat facilisis ac faucibus vitae nulla in augue nullam neque.
        </div>
        <div>
          Lorem ipsum dolor sit amet consectetur. Ornare id amet pellentesque at vitae metus amet. Placerat facilisis ac faucibus vitae nulla in augue nullam neque.
        </div>
      </div>
    </template>
    <template v-slot:button2>
      <q-btn
        color="primary"
        label="En savoir plus"
        class="q-mt-md"
      />
    </template>
    <template v-slot:image2>
      <q-img src="../assets/card2.png" />
    </template>
  </HomeCard>
  <div class="q-py-xl"></div>
</template> -->

<style scoped>
.title{
  font-family: 'Kanit';
  font-style: normal;
  font-weight: 400;
  font-size: 45px;
  line-height: 55px;
  text-transform: uppercase;
  color: white;
}

@media screen and (max-width: 910px) {
  .title{
      font-size: 30px;
      line-height: 40px;
  }
}

</style>