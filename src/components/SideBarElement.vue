<template>
    <div class="d-flex mb-3">
        <span class="material-symbols-outlined"> {{ icon }} </span>
        <p class="mx-2 my-0"> {{ libelle }} </p>
    </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';

defineProps({
    libelle: String,
    icon: String,
})

</script>

<style></style>