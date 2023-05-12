<script setup>
import employee1 from '../assets/employee/employee1.png';
import employee2 from '../assets/employee/employee2.png';
import employee3 from '../assets/employee/employee3.png';
import employee4 from '../assets/employee/employee4.png';
import employee5 from '../assets/employee/employee5.png';
import employee6 from '../assets/employee/employee6.png';

const employees = [
    {
        name: 'Jean-François Lévesque',
        job: 'Président',
        image: employee1
    },
    {
        name: 'Jean-François Lévesque',
        job: 'Président',
        image: employee2
    },
    {
        name: 'Jean-François Lévesque',
        job: 'Président',
        image: employee3
    },
    {
        name: 'Jean-François Lévesque',
        job: 'Président',
        image: employee4
    },
    {
        name: 'Jean-François Lévesque',
        job: 'Président',
        image: employee5
    },
    {
        name: 'Jean-François Lévesque',
        job: 'Président',
        image: employee6
    },
]
</script>

<template>
    <v-container>
    <v-row class="text-white justify-center">
        <v-col v-for="(employee, index) in employees" :key="index" cols="8" md="4">
            <v-card class="my-card col">
            <v-card-text>
                <v-img :src="employee.image" />
            </v-card-text>
            <v-card-text>
                <div class="text-h6">{{ employee.name }}</div>
                <div class="q-py-md">{{ employee.job }}</div>
            </v-card-text>
            </v-card>
        </v-col>
    </v-row>
</v-container>  
    <div class="q-pa-md"></div>
</template>
    
<style scoped>
.my-card{
    max-width: 425px;
    border-radius: 16px;
    background: transparent;
}
</style>