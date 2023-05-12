<script setup lang="ts">
    import { ref } from 'vue'

    //Register
    const nom = ref(null);
    const email = ref(null);
    const password = ref(null);
    const confirmPassword = ref(null);
    
    function registerForm() {
        //authStore.addUser(nom.value, email.value, password.value);
        return 1;
    }
</script>

<template>
    <div>
        <h4 class="text-blue-grey-2 text-center">Register</h4>
        <form @submit="registerForm">
            <q-input class="bg-blue-grey-2" label="Nom" v-model="nom"/>
            <q-input class="bg-blue-grey-2" label="Email" v-model="email"/>
            <q-input class="bg-blue-grey-2" label="Mot de passe" v-model="password"/>
            <q-input class="bg-blue-grey-2" label="Confirmer le mot de passe" v-model="confirmPassword"/>

            <q-btn class="bg-blue-grey-2" label="Submit" type="submit"/>
        </form>
    </div>
</template>