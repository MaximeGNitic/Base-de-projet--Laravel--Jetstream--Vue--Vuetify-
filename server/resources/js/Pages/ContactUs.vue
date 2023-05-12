<script setup lang="ts">
import TitleComponent from '../Components/TitleComponent.vue';
import ContactForm from '../Components/Contact/ContactForm.vue';
// import ContactInfo from 'src/components/Contact/ContactForm.vue';
</script>

<template>
    <TitleComponent>
      <template v-slot:upTitle>
        Nous joindre
      </template>
    </TitleComponent>
  <div class="q-py-lg"></div>
  <ContactForm />
  <div class="q-py-lg"></div>
</template>


