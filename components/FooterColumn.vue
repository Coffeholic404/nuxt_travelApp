<template>
    <div class="flex flex-col gap-5">
        <h4 class="bold-18 whitespace-nowrap">
            {{ props.title }}
        </h4>
        <slot />
    </div>
</template>

<script setup lang="ts">
const props = defineProps({
  title: {
    require: true,
    type: String
  }
})

</script>

<style scoped>

</style>