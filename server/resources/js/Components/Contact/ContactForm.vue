<script setup lang="ts">
import { ref, computed } from 'vue'


const name = ref('')
const phone = ref(null)
const email = ref('')
const text = ref('')

const onSubmit = (evt: Event) => {
  evt.preventDefault()
    console.log('submitted')
}

const onReset = (evt: Event | undefined) => {
    evt && evt.preventDefault()
    name.value = ''
    phone.value = null
    email.value = ''
}
</script>

<template>
    <div class="column flex-center text-white">
        <div class="col-5 flex flex-center text-h3 text-center text-h4-md">
            Vous avez une question?
        </div>
        <div class="q-py-sm"></div>
        <div class="row q-pa-md" style="width:75%">

            <q-form
            @submit="onSubmit"
            @reset="onReset"
            class="col q-gutter-md"
            >
            <div class="row">
                <!-- :rules="[ val => val && val.length > 0 || 'Please type something']" -->
                <q-input
                class="col"
                filled
                v-model="name"
                label="Nom complet"
                input-class="text-white"
                :label-color="name ? 'primary' : 'white'"
                style="background-color: rgba(255, 255, 255, 0.15);
                text-decoration: underline white;
                "
                />
                <!-- :rules="[ val => val && val.length > 0 || 'Please type something']" -->
                <q-input
                class="col q-ml-md"
                filled
                v-model="phone"
                label="Numéro de téléphone"
                input-class="text-white"
                :label-color="name ? 'primary' : 'white'"
                style="background-color: rgba(255, 255, 255, 0.15);
                color: azure;
                "
                />
                </div>
                <div class="q-px-md"></div>

                <q-input
                class="col"
                filled
                v-model="email"
                label="Adresse courriel"
                input-class="text-white"
                :label-color="name ? 'primary' : 'white'"
                style="background-color: rgba(255, 255, 255, 0.15);
                color: azure;
                "
                />

                <div>
                    <q-input
                    v-model="text"
                    label="Que pouvez-nous faire pour vous?"
                    filled
                    type="textarea"
                    :label-color="name ? 'primary' : 'white'"
                    style="background-color: rgba(255, 255, 255, 0.15);"
                    />
                </div>
            </q-form>

        </div>
    </div>
</template>