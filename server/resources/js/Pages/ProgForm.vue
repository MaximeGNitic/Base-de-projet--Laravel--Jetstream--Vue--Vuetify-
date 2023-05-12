<script setup lang="ts">
import TitleComponent from '../Components/TitleComponent.vue';
import TextContent from '../Components/TextContent.vue';
import CardLogo from '../Components/CardLogo.vue';
import WhyProject from '../Components/WhyProject.vue';
</script>

<template>
    <TitleComponent>
        <template v-slot:upTitle>
            Programme de formation sur mesure Découverte
        </template>
    </TitleComponent>
    <div class="q-py-xl"></div>
    <TextContent>
        <template v-slot:underTitle>
            Depuis 2015, l’équipe de Minopro-Cree a travaillé sur différents programmes de formations afin d’intégrer de nouveaux travailleurs diplômés cris dans le milieu industriel. Étant au fait des défis quotidiens, Minopro-Cree se veut être une aide complémentaire à votre équipe pour combler vos besoins de main d’oeuvre. Quoique Minopro-Cree priorisera toujours la diplomation, le programme de formation sur mesure Découverte a été fondé dans le but d’offrir une formation complète qui aborde toutes les connaissances nécessaires qu’auront besoins votre future maind’oeuvre afin d’être polyvalente et autonome. Minopro et Minopro-Cree croient que la formation continue et intégrée est désormais un élément clé important à ajouter à nos stratégies pour favoriser la pérennité et la stabilité de main-d’oeuvre au sein des organisations.
        </template>
    </TextContent>
    <div class="q-py-xl"></div>
    <CardLogo>
        <template v-slot:cardTitle>
            Le programme découverte
        </template>
        <template v-slot:cardUnderTitle>
            Le programme Découverte se voit comme une formation unique en milieu de travail permettant à votre organisation de recruter, former et intégrer une main-d’oeuvre autochtone selon vos besoins bien précis. Les apprenants des cohorte auront l’opportunité grâce à un formateur d’expérience dédié à eux de se familiariser dans vos installations tout en apprenant un métier avec des notions théoriques et pratiques. L’un des objectifs de ce programme est de donner l’occasion aux gens des communautés de développer des aptitudes dans le secteur industriel et d’accéder à un emploi de qualité par la suite.
        </template>
        <template v-slot:listTitle>
            Les avantages
        </template>
        <template v-slot:listContent>
            <ul>
                <li>Formation de 6 mois</li>
                <li>Formation en classe et en entreprise</li>
                <li>Formation théorique et pratique</li>
                <li>Formation sur mesure</li>
                <li>Formation en groupe</li>
                <li>Formation en entreprise</li>
                <li>Formation en entreprise</li>
                <li>Formation en entreprise</li>
            </ul>
        </template>
    </CardLogo>
    <div class="q-py-xl"></div>
    <div>
       <WhyProject />
    </div>
    <div class="q-py-xl"></div>
    <TextContent>
        <template v-slot:upTitle>
            L’implantation
        </template>
        <template v-slot:underTitle>
            L’implantation d’un programme Découverte nécessite une préparation adéquate afin d’offrir et monter une formation répondant à des exigences bien précises. Le programme se réalise dans différentes phases afin d’assurer le succès de la formation.
        </template>
        <template v-slot:listContent>
            <ul>
                <li>Phase d’élaboration</li>
                <li>Phase de recrutement et de visibilité</li>
                <li>Phase de formation</li>
                <li>Phase d’intégration</li>
                <li>Phase suivi post-formation</li>
            </ul>
        </template>   
    </TextContent>
    <div class="q-py-xl"></div>
</template>