<script setup lang="ts">
import { type ChaussureSvg } from '@/types-svg';
import VueProfil from '@/components/VueProfil.vue';
import VueDessus from '@/components/VueDessus.vue';
import FormSvg from '@/components/FormSvg.vue';
import FormImages from '@/components/FormImages.vue';
import BasketProfil from "../components/BasketProfil.vue";
import type { Basket } from "../types";
const exemple0: Basket = {
  semelle: "#FF0000",
  empeigne: "#FFFFFF",
  pointe: "#FFFFFF",
  oeillet: "#FFFFFF",
  bande: "#00FF00",
  languette: "#FFFFFF",
  lacet: "#00FF00",
  trimestre: "#FFFFFF",
};
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
    <FormImages />

      <section>
    <h1 class="text-2xl">Exemples de Baskets</h1>
    <div class="flex flex-wrap gap-2">
      <div class="w-64">
        <RouterLink
          :to="{
            name: '/basket/exemple/[data]',
            params: { data: JSON.stringify(exemple0) },
          }"
        >
          <BasketProfil class="w-64" v-bind="exemple0" />
        </RouterLink>
      </div>
    </div>
  </section>


</template>