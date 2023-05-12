<script setup>
import TitleComponent from '../Components/TitleComponent.vue';
import TextContent from '../Components/TextContent.vue';
import ButtonPrimary from '../Components/ButtonPrimary.vue';
import ProcessCard from '../Components/ProcessCard.vue';
import WorkListCard from '../Components/WorkListCard.vue';
</script>

<template>
    <TitleComponent>
        <template v-slot:upTitle>
            Service de main-d’oeuvre qualifiée
        </template>
        <template v-slot:underTitle>
            Besoin de main-d’oeuvre pour une période de courte ou longue durée ? Nous sommes la référence en capital humain dans le domaine industriel.
        </template>
    </TitleComponent>

    <div class="q-py-xl"></div>
    <div class="q-py-xl"></div>

    <TextContent>
        <template v-slot:upTitle>
            Qu’est-ce que le service de main-d’oeuvre qualifiée ?
        </template>
        <template v-slot:underTitle>
            Notre service de main-d’oeuvre qualifiée vous offre une banque de candidats selon vos besoins. Nous dénicherons LA bonne personne pour vous. L’expérience en tant qu'ingénieur de procédés des membres de notre équipe ainsi que notre équipe en ressources humaines et communications, nous permettent de dénicher les meilleurs candidats pour vos besoins de main-d'oeuvre en réduisant le risque d’embaucher un candidat qui ne s’adapterait pas convenablement. Nous savons exactement en quoi consistent les postes et les tâches à réaliser, ce qui nous aide à bien sélectionner et préparer votre future main-d'oeuvre. Chaque année, plusieurs partenaires choisissent Minopro pour les différents avantages que procure notre service.
        </template>
        <template v-slot:listContent>
            <ul>
                <li>Une banque de candidat qualifiée</li>
                <li>La gestion globale du candidat</li>
                <li>L’économie de temps</li>
                <li>Un recrutement actif et continue</li>
                <li>La promotion de votre marque employeur</li>
                <li>Un réseau de travailleurs qualifié et intéressant</li>
            </ul>
        </template>
        <template v-slot:underTitle2>
            Au fil des années, nous avons développé une relation solide avec les institutions d'enseignement. Minopro visite pour vous les écoles afin de vous représenter directement auprès de la future main-d'oeuvre. Ce positionnement nous permet de repérer, à la source, les candidats répondant le mieux au profil de la tâche que vous désirez accomplir. De plus, nous avons également mis en place une stratégie de visibilité et de recrutement efficace sur les réseaux sociaux qui vient supporter nos démarches plus traditionnelles afin de rejoindre un bassin de travailleurs plus varié. Ainsi, vos équipes peuvent se concentrer sur leur travail, car Minopro s'occupe de dénicher vos futurs talents via différents canaux de recrutement ! Notre objectif est de vous offrir une main-d'oeuvre qualifiée, motivée et fiable dans une optique d’intégration durable.
        </template>
    </TextContent>

    <div class="q-py-md"></div>

    <div class="flex flex-center">
        <div class="flex flex-start" style="width: 75%;">
            <ButtonPrimary label="Trouver un employé" />
        </div>
    </div>

    <div class="q-py-xl"></div>





    <div>
        <WorkListCard>
            <template v-slot:image>
                <q-img src="../assets/card.png"/>
            </template>

            <template v-slot:title>
                <div class="title flex flex-center">
                    Nos domaines d’expertise
                </div>
            </template>
            <template v-slot:list>
                <ul class="col">
                    <li>Journaliers</li>
                    <li>Opérateurs machinerie fixe</li>
                    <li>Opérateurs machinerie lourde</li>
                    <li>Mécaniciens industriels</li>
                    <li>Techniciens en métallurgie</li>
                    <li>Commis</li>
                    <li>Superviseurs</li>
                    <li>Métallurgistes</li>
                    <li>Techniciens en chimie analytique</li>
                </ul>
            </template>
            <template v-slot:button>
                <div style="width: 75%;">
                <q-btn color="white" text-color="black" label="Voir les offres d’emploi" class="q-px-lg" />
                </div>
            </template>
            <!-- <template v-slot:list>
                <TextContent>

                </TextContent>
            </template> -->
        </WorkListCard>
    </div>
    




    <div class="q-py-xl"></div>
    <div class="flex flex-center q-gutter-md">
        <div class="row" style="width: 75%;">
            <ProcessCard class="col-12 col-md">
                <template v-slot:number>01</template>
                <template v-slot:title>
                    <div>
                        Prise en compte des besoins
                    </div>
                    
                </template>
                <template v-slot:description>
                    Première rencontre visant à déterminer le mandat et obtenir toutes les informations nécessaires pour la recherche de candidats.
                </template>
            </ProcessCard>
            <div class="q-pa-md"></div>
            <ProcessCard class="col-12 col-md">
                <template v-slot:number>02</template>
                <template v-slot:title>Phase de recrutement</template>
                <template v-slot:description>
                    Première rencontre visant à déterminer le mandat et obtenir toutes les informations nécessaires pour la recherche de candidats.
                </template>
            </ProcessCard>
        </div> 
        <div class="row" style="width: 75%;">
            <ProcessCard class="col-12 col-md">
                <template v-slot:number>03</template>
                <template v-slot:title>Phase d’entrevue</template>
                <template v-slot:description>
                    Première rencontre visant à déterminer le mandat et obtenir toutes les informations nécessaires pour la recherche de candidats.
                </template>
            </ProcessCard>
            <div class="q-pa-md"></div>
            <ProcessCard class="col-12 col-md">
                <template v-slot:number>04</template>
                <template v-slot:title>Phase de sélection</template>
                <template v-slot:description>
                    Première rencontre visant à déterminer le mandat et obtenir toutes les informations nécessaires pour la recherche de candidats.
                </template>
            </ProcessCard>
        </div>
        <div class="row" style="width: 75%;">
            <ProcessCard class="col-12 col-md">
                <template v-slot:number>05</template>
                <template v-slot:title>Phase d’embauche et d’intégration</template>
                <template v-slot:description>
                    Première rencontre visant à déterminer le mandat et obtenir toutes les informations nécessaires pour la recherche de candidats.
                </template>
            </ProcessCard>
            <div class="q-pa-md"></div>
            <ProcessCard class="col-12 col-md">
                <template v-slot:number>06</template>
                <template v-slot:title>Suivi en milieu de travail</template>
                <template v-slot:description>
                    Première rencontre visant à déterminer le mandat et obtenir toutes les informations nécessaires pour la recherche de candidats.
                </template>
            </ProcessCard>
        </div>
    </div>
    <div class="q-py-md"></div>
    <div class="flex flex-center">
        <div class="flex flex-start" style="width: 75%;">
            <ButtonPrimary label="Avoir du soutien" />
        </div>
    </div>
    <div class="q-py-xl"></div>
</template>

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
