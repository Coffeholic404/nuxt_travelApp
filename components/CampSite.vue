<template>
    <div :class="` h-full w-full min-w-[1100px] ${props.backgroundImage} bg-cover bg-no-repeat lg:rounded-r-5xl 2xl:rounded-5xl`">
        <div class="flex h-full flex-col items-start justify-between p-6 lg:px-20 lg:py-10">
            <div class=" flexCenter gap-4">
                <div class=" rounded-full bg-green-50 p-4">
                    <NuxtImg 
                    src="folded-map.svg"
                    alt="Map"
                    width="28"
                    height="28"
                    />
                </div>
                <div class=" flex flex-col gap-1">
                    <h4 class=" bold-18 text-white">{{ props.title }}</h4>
                    <p class="regular-14 text-white">{{ props.subtitle }}</p>
                </div>
            </div>

            <div class="flexCenter gap-6">
                <span  class=" flex -space-x-4 overflow-hidden">
                <NuxtImg 
                v-for="people in peopleUrl"
                :src="`${people}`"
                :key="people"
                alt="person"
                height="52"
                width="52"
                class=" inline-block h-10 w-10 rounded-full"
                />
            </span>
            <p class="bold-16 md:bold-20 text-white"> {{ props.peopleJoined }} </p>
            </div>

        </div>
    </div>
</template>

<script setup lang="ts">
import { PEOPLE_URL } from '~/constants';

interface CampProps {
    backgroundImage: string
    title: string
    subtitle: string
    peopleJoined: string
}
const props = defineProps<CampProps>()
const peopleUrl = PEOPLE_URL.map((url) => url)
</script>

<style scoped>

</style>