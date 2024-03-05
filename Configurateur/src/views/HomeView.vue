<script setup lang="ts">
import { ChaussureSvg } from '@/types-svg';
import VueProfil from '@/components/VueProfil.vue';
import VueDessus from '@/components/VueDessus.vue';
import FormSvg from '@/components/FormSvg.vue';

</script>

<template>
    <h1>Bonjour</h1>
    <p>Chaussures :</p>
    <VueProfil />
    Vue du dessus :
    <div class="w-[500px] mt-4 ml-3">
    <VueDessus />
    </div>
    <FormSvg />
</template>