<script setup lang="ts">
// import TitleComponent from 'src/components/AboutUs/TitleComponent.vue';
import TitleComponent from '../Components/TitleComponent.vue';
import CardLogo from '../Components/CardLogo.vue';
import WorkerCard2 from '../Components/WorkerCard2.vue';
import TextContent from '../Components/TextContent.vue';
import OurTeam from '../Components/OurTeam.vue';
</script>

<template>
  <TitleComponent>
    <template v-slot:upTitle>
      Qui sommes-nous ?
    </template>
  </TitleComponent>

  <div class="q-py-lg"></div>

  <div class="column flex-center">
    <div class="col" style="width: 75%;">
        <q-img src="../assets/9AboutUs.png"  />
    </div>
  </div>

  <div class="q-py-lg"></div>

  <div>
    <UnderTitle />
  </div>

  <div class="q-py-xl"></div>

  <CardLogo>
    <template v-slot:cardTitle>
      Minopro-cree
    </template>
    <template v-slot:cardUnderTitle>
      À travers toutes nos activités, Minopro-Cree a pour mission quotidienne de travailler en collaboration et de s’engager au sein des communautés de Eeyou Istchee dans l’atteinte d’objectifs communs: recruter, former et intégrer une main-d’œuvre crie dans les milieux industriels situés sur le territoire Eeyou Istchee. En plus d’offrir un service de main-d’œuvre qualifiée, nous avons mis en place un programme de formation dédiée aux gens des communautés cris dans le but de les former et de les intégrer les milieux de travail. Nos formations ne sont pas simplement théoriques pour faire connaître le milieu industriel, mais conçues pour préparer les gens sur le terrain à de vrais emplois sur les lieux de travail.
      Bien que Minopro-Cree travaille en collaboration avec les communautés, une grande portion de nos employés viennent de partout. Ce sont donc tous les travailleurs du Québec, de l’Ontario [AH1] et d’ailleurs qui sont invités à postuler sur les offres d’emploi situés sur le territoire Eeyou Istchee.
      [AH1]On a déjà eu des gens de l'extérieur de ces 2 provinces (ex maritimes) qui ont travaillé pour nous
    </template>
  </CardLogo>

  <div class="py-16"></div>

  <div class="flex flex-center text-white">
        <div class="row justify-center" style="width: 75%;">
      <WorkerCard2 class="col-lg-4 col-12">
        <template v-slot:Title>
          Mission
        </template>
        <template v-slot:Description>
          Être un partenaire de réussite récurrent dans l’intégration durable, la rétention, la valorisation et la formation de la main d’œuvre qualifiée dans le milieu industriel.
        </template>
      </WorkerCard2>
      <WorkerCard2 class="col-lg-4 col-12">
        <template v-slot:Title>
          Vision
        </template>
        <template v-slot:Description>
            <p>Être la référence en support intégrée du capital humain.</p>
            <p>Être engagé dans l’accroissement du développement des communautés touchées.</p>
            <p>Utiliser les forces de notre partenariat cri afin de développer un modèle d'affaires durable et l’étendre à d’autres nations autochtones.</p>
        </template>
      </WorkerCard2>
      <WorkerCard2 class="col-lg-4 col-12">
        <template v-slot:Title>
          Valeurs
        </template>
        <template v-slot:Description>
            <p>Engagement</p>
            <p>Innovation sociale</p>
            <p>Esprit d'équipe</p>
            <p>Satisfaction de nos partenaires</p>
        </template>
      </WorkerCard2>
    </div>
  </div>
  <div class="q-py-lg"></div>

  <TextContent>
    <template v-slot:upTitle>
      Notre expertise
    </template>
    <template v-slot:underTitle>
      Notre expertise se traduit par l’expérience diversifiée acquise au fil des années par chacun des membres de notre équipe.
      L’une de nos forces en tant qu’organisation est d’avoir un champ d’expertise diversifié dans le milieu industriel, ce qui nous permet d’accompagner nos partenaires dans les différents besoins opérationnels. Avec le temps, notre expertise acquise en milieu de travail s’est combinée à des ressources en capital humain et en communications / marketing qui nous permettent aujourd’hui d’offrir une expérience client répondant vite et de manière personnalisée aux besoins.
    </template>
  </TextContent>

  <div class="q-py-lg"></div>
  <div>
    <OurTeam />
  </div>
  <div class="q-py-lg"></div>

</template>


