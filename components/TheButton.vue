<template>
    <button
    :class="`flexCenter gap-3 rounded-full border ${props.variant}`"
    :type="props.type">
        <NuxtImg v-if="props.icon"
        :src="props.icon"
        :alt="props.title"
        width="24"
        height="24"
        >
        </NuxtImg>
        <label class="bold-16 whitespace-nowrap">{{ props.title }}</label>
    </button>
</template>

<script setup lang="ts">
interface ButtonProps {
    type: 'button' | 'submit'
    title: string
    icon?: string
    variant: 'btn_dark_green'
}
const props = defineProps<ButtonProps>()
</script>

<style scoped>

</style>