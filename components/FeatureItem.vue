<template>
    <li class=" flex w-full flex-1 flex-col items-start" v-for="feature in features">
        <div class=" rounded-full p-4 lg:p-7 bg-green-50">
            <NuxtImg 
            :src="`../public${feature.icon}`"
            alt="map"
            width="28"
            height="28"
            />
        </div>
        <h2 class=" bold-20 lg:bold-32 mt-5 capitalize">
            {{ feature.title }}
        </h2>
        <p class=" regular-16 mt-5 bg-white/80 text-gray-30 lg:mt-[30px] lg:bg-none">{{ feature.description }}</p>
    </li>
</template>

<script setup lang="ts">
//interface featureProps{
//     title:string
//     icon:string
//     variant:string
//     description:string
// }
import { FEATURES } from '~/constants';


const features = FEATURES.map((feat) => feat);


</script>

<style scoped>

</style>