<template>
    <section class="flex-col flexCenter overflow-hidden bg-feature-bg bg-center bg-no-repeat py-24">
        <div class="max-container padding-container relative w-full flex justify-end">

            <div class="flex flex-1 lg:min-h-[900px]">
                <NuxtImg 
                src="../public/phone.png"
                alt="phone"
                width="440"
                height="1000"
                class="feature-phone"
                />
            </div>

            <div class=" z-20 flex w-full flex-col lg:w-[60%]">
                <div class=" relative">
                    <NuxtImg 
                    src="../public/camp.svg"
                    alt="camp"
                    width="50"
                    height="50"
                    class=" absolute left-[-5px] top-[-28px] w-10 lg:w-[50px]"
                    />
                    <h2 class="bold-40 lg:bold-64">Our Features</h2>
                </div>
                <ul class=" mt-10 grid gap-10 md:grid-cols-2 lg:mt-20 lg:gap-20">
                    <FeatureItem />
                </ul>
            </div>
        </div>

    </section>
</template>

<script setup lang="ts">

</script>

<style scoped>

</style>