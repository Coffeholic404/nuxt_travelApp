<template>
    <footer class="flexCenter mb-24">
        <div class="padding-container max-container flex w-full flex-col gap-14">
            <div class="flex flex-col items-start justify-center gap-[10%] md:flex-row">
                <NuxtLink to="/" class="mb-10">
                    <NuxtImg 
                    src="hilink-logo.svg"
                    alt="logo"
                    width="74"
                    height="29"
                    />
                </NuxtLink>

                <div class="flex flex-wrap gap-10 sm:justify-between md:flex-1">
                    <FooterColumn
                    v-for="column in footerLinks"
                    :title="column.title"
                    >
                    <ul class=" regular-14 flex flex-col gap-4 text-gray-30">
                        <NuxtLink to="/" v-for="link in column.links" :key="link">
                            {{ link }}
                        </NuxtLink>
                    </ul>
                    </FooterColumn>

                    <div class="flex flex-col gap-5">
                        <FooterColumn
                        :title="contactInfo.title"
                        >
                        <NuxtLink
                        to="/"
                        v-for="link in contactInfo.links" key="link"
                        class=" flex gap-4 md:flex-col lg:flex-row"
                        >
                        <p class=" whitespace-nowrap">
                            {{ link.label }}:
                        </p>
                        <p class="medium-14 whitespace-nowrap text-blue-70">{{ link.value }}</p>
                        </NuxtLink>
                        </FooterColumn>
                    </div>

                    <div class="flex flex-col gap-5">
                        <FooterColumn
                        :title="socials.title"
                        >
                        <ul class="regular-14 flex gap-4 text-gray-30">
                            <NuxtLink
                            v-for="link in socials.links"
                            :key="link"
                            to="/"
                            >
                            <NuxtImg 
                            :src="link"
                            alt="logo"
                            width="24"
                            height="24"
                            />
                            </NuxtLink>

                        </ul>
                        </FooterColumn>

                    </div>

                </div>

            </div>
            <div class="border bg-gray-20"/>
            <p class="regular-14 w-full text-center text-gray-30">2024 Hilink | All right reserved</p>
        </div>
    </footer>
</template>

<script setup lang="ts">
import { FOOTER_CONTACT_INFO, FOOTER_LINKS, SOCIALS } from '~/constants';

const footerLinks = FOOTER_LINKS.map((column) => column)
const contactInfo = FOOTER_CONTACT_INFO
const socials = SOCIALS
</script>

<style scoped>

</style>