<script setup lang="ts">
const emit = (event : string) => {
    console.log(event);
}
</script>

<template>
    <q-btn
        class="primary-btn q-px-lg"
        style="border-radius: 12px;"
        @click="emit('click')"
    />
</template>

<style>
.primary-btn{
    font-family: 'Kanit';
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 27px;
    color: #1D1D1B;
    background-color: white;
}
</style>