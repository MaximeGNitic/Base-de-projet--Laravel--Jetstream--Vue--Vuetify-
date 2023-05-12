<script setup lang="ts">
import TitleComponent from '../Components/TitleComponent.vue';
import TextContent from '../Components/TextContent.vue';
import ButtonPrimary from '../Components/ButtonPrimary.vue';
</script>

<template>
    <TitleComponent>
        <template v-slot:upTitle>
            Nos Soutien en usine
        </template>
    </TitleComponent>
    <TextContent>
        <template v-slot:underTitle>
            Les connaissances et le bagage d’expérience acquise à travers les années et les différents mandats font de nous l’accompagnateur par excellence dans le démarrage de votre usine et dans l’accompagnement. L’accompagnement en usine offre différents avantages tels que :
        </template>
        <template v-slot:listContent>
            <ul>
                <li>Aide au démarrage, montée en puissance et production commerciale;</li>
                <li>Production de documents contrôlés;</li>
                <li>Mise en place d’une structure de suivi de la formation interne;</li>
                <li>Projet clé en main de création et gestion d'équipe d'opération.</li>
            </ul>
        </template>
        <template v-slot:underTitle2>
            Si vous manquez de ressources pour mener à bien vos projets dans votre usine ou bien dans votre laboratoire, n'hésitez pas à nous contacter.
        </template>
    </TextContent>

    <div class="q-py-md"></div>
    <div class="flex flex-center">
        <div class="flex flex-start" style="width: 75%;">
            <ButtonPrimary label="Avoir du soutien" />
        </div>
    </div>

    <div class="q-py-xl"></div>

    <TextContent>
        <template v-slot:upTitle>
            Nos différents mandats accomplit
        </template>
        <template v-slot:listContent>
            <ul>
                <li>Support à l'opération</li>
                <li>Préparation au démarrage d'usine (Operation Rediness Plan);</li>
                <li>Démarrage et opération d'usines pilotes</li>
                <li>Support au démarrage d'usines</li>
                <li>Essais métallurgiques et optimisation de procédés au concentrateur</li>
            </ul>
        </template>
    </TextContent>
    <div class="q-py-xl"></div>
    <TextContent>
        <template v-slot:upTitle>
            Documentation contrôlée
        </template>
        <template v-slot:underTitle>
            Pour l’avoir implanté dans plusieurs usines, Minopro à l’expertise pour mettre en place une structure pouvant supporter la formation par compagnonnage. L’objectif est d’offrir aux apprentis un processus structuré et organisé de formation propre à développer les compétences recherchées (connaissances, habiletés et attitude) par poste d’opération.
            Au niveau de la structure de documentation, nous faisons la mise en place d’un processus de création, révision et approbation de la documentation (procédures, routes d’inspection, formation…). Nous faisons également la rédaction de guides de compagnonnage (guide de formation).
        </template>
        <template v-slot:listTitle>
            <div class="q-py-md">Les avantages de la documentation et de la formation ;</div>
        </template>
        <template v-slot:listContent>
            <ul>
                <li>Analyse des processus et des méthodes de travail</li>
                <li>Diminuer les risques d’incidents et d’accidents</li>
                <li>Formation uniforme dans le temps</li>
                <li>Uniformiser les façons de faire pour les équipes (poste, tâches)</li>
                <li>Réduit les risques d’erreur</li>
                <li>Augmente le niveau de connaissance des équipes</li>
                <li>Intégration d’un système efficace de suivi des formations, des compétences et de la documentation contrôlée</li>
            </ul>
        </template>
    </TextContent>
    <div class="q-py-xl"></div>
    <TextContent>
        <template v-slot:upTitle>
            Nos différents mandats accomplit
        </template>
        <template v-slot:listContent>
            <ul>
                <li>Écriture de procédures d'opération</li>
                <li>Mise en place d’une numérotation de la documentation contrôlée (Clé documentaire)</li>
                <li>Mise en place d’un processus de rédaction, révision et approbation de la documentation contrôlée.</li>
                <li>Création des guides de formation par poste de travail. (document, risque, criticité des documents).</li>
                <li>Mise en place d'une structure de formation pour l'usine.</li>
                <li>Intégration d’un système efficace de suivi des formations, des compétences et de la documentation contrôlée.</li>
                <li>Mise à jour de la documentation contrôlée.</li>
            </ul>
        </template>
    </TextContent>
    <!-- <div>
        <SoutienUsine />
    </div> -->
    <div class="q-py-xl"></div>
</template>