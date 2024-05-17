<template>
    <div class="px-1 py-2 d-flex flex-column ">
        <img :src="image" alt="image du produit" style="height: 130px; width: 130px; object-fit: cover;">
        <p class="fw-lighter text-center my-0 mb-2" style="font-size: 15px;">
            {{ nom }}
        </p>
    </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';

defineProps({
    image: String,
    nom: String
})

</script>

<style></style>