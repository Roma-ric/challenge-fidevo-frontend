<template>
    <div class="px-1 py-2 d-flex flex-column position-relative">
        <div class="d-flex flex-column justify-content-end align-items-end position-absolute p-1 favorite">
            <span
                class="material-symbols-outlined card pt-1 d-flex justify-content-center align-items-center rounded rounded-circle"
                style="width: 35px; height: 35px;"> favorite </span>
        </div>
        <img :src="image" alt="image du produit" style="height: 200px; object-fit: cover;">
        <div class="d-flex align-items-center">
            <h6 class="fw-bold text-start m-0" style="color: green;"> Now ${{ nouveau_prix }} </h6>
            <p v-if="ancien_prix" class="mx-2 fw-lighter text-secondary text-start text-decoration-line-through my-0"
                style="font-size: 15px;"> ${{ ancien_prix }} </p>
        </div>
        <p class="fw-lighter text-start my-0 mb-2">
            {{
                description && description.length > 38
                    ? (() => {
                        const spaceBefore = description.lastIndexOf(' ', 38);
                        const spaceAfter = description.indexOf(' ', 38);
                        const closestSpace = (spaceAfter === -1 || (spaceBefore !== -1 && 38 - spaceBefore < spaceAfter - 38)) ?
                            spaceBefore : spaceAfter; return description.slice(0, closestSpace) + "...";
                    })() : description }} </p>
                <div v-if="button == 1" class="d-flex justify-content-start ">
                    <button 
                        class="m-0 btn text-dark border-dark rounded rounded-pill bg-light fw-lighter">
                        Options
                    </button>
                </div>
                <div v-if="button == 2" class="d-flex justify-content-start ">
                    <button 
                        class="m-0 btn text-dark border-dark rounded rounded-pill bg-light fw-lighter">
                        +
                        Add
                    </button>
                </div>
    </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';

defineProps({
    image: String,
    ancien_prix: Number,
    nouveau_prix: Number,
    description: String,
    button: Number
})
</script>

<style>
@media (max-width: 767px) {
    .favorite {
        left: 125px
    }
}

@media (min-width: 768px) and (max-width: 991px) {
    .favorite {
        left: 190px
    }
}

@media (min-width: 992px) {
    .favorite {
        left: 170px
    }
}
</style>