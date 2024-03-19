<template>
  <nav class=" flexBetween max-container padding-container relative z-30 py-5">
    <NuxtLink to="/">
        <NuxtImg 
        src="../public/hilink-logo.svg"
        alt="Logo"
        width="74"
        height="29"
        />
    </NuxtLink>
    <ul class=" hidden h-full gap-12 lg:flex">
      <li v-for="link in navItems" key="link.key"
      class=" reqular-16 text-gray-50 flexCenter cursor-pointer pb-1.5 transition-all hover:font-bold"
      >
        <NuxtLink to="link.href">
          {{ link.label }}
      </NuxtLink>
      </li>
    </ul>

    <div class="lg:flexCenter hidden">
      <TheButton 
      type="button"
      title="Login"
      icon="../public/user.svg"
      variant="btn_dark_green"
      
      />
    </div>

    <NuxtImg 
    src="../public/menu.svg"
    alt="Menu"
    width="32"
    height="32"
    class=" inline-block cursor-pointer lg:hidden"
    />
  </nav>
</template>

<script setup lang="ts">
import { NAV_LINKS } from '~/constants';
const navItems = NAV_LINKS.map((link) => link);
</script>
