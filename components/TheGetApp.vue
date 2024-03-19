<template>
    <section class="flexCenter w-full flex-col pb-[100px]">
        <div class="get-app">
            <div class=" z-20 flex flex-1 flex-col items-start justify-center w-full gap-12">
                <h2 class="bold-40 lg:bold-64 xl:max-w-[320px]">Get For Free Now</h2>
                <p class="regular-16 text-gray-10">Available on IOS And Android</p>
                <div class="flex w-full flex-col gap-3 whitespace-nowrap xl:flex-row">
                    <TheButton 
                    type="button"
                    title="Download App"
                    icon="/apple.svg"
                    variant="btn_white"
                    />
                    <TheButton 
                    type="button"
                    title="Play Store"
                    icon="/android.svg"
                    variant="btn_dark_green_outline"
                    />
                </div>
            </div>
            <div class="flex flex-1 items-center justify-end">
                <NuxtImg
                src="phones.png"
                alt="phone"
                width="550"
                height="870"
                />
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">

</script>

<style scoped>

</style>