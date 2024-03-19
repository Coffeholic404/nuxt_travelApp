<template>
  <section
    class="2xl:max-container relative flex flex-col py-10 lg:mb-10 lg:py-20 xl:mb-20"
  >
    <div
      class="hide-scrollbar flex h-[340px] w-full items-start justify-start gap-8 overflow-x-auto lg:h-[400px] xl:h-[640px]"
    >
      <CampSite
        backgroundImage="bg-bg-img-1"
        title="Putuk Truno Camp"
        subtitle="Prigen, Pasuruan"
        peopleJoined="30+ Joined"
      />
      <CampSite
        backgroundImage="bg-bg-img-2"
        title="Mountain View Camp"
        subtitle="Somewhere In The Wilderness"
        peopleJoined="40+ Joined"
      />
    </div>

    <div class="flexEnd mt-10 px-6 lg:-mt-60 lg:mr-6">
        <div class=" bg-green-50 p-8 lg:max-w-[500px] xl:max-w-[734px] xl:rounded-5xl xl:px-16 xl:py-20 relative w-full overflow-hidden rounded-3xl">
            <h2 class=" regular-24 md:regular-32 2xl:regular-64 capitalize text-white">
               <strong>Feeling Lost </strong>And Not Knowing The Way? 
            </h2>
            <p class=" regular-14 xl:regular-16 mt-5 text-white">Starting from the anxiety of the climbers when visiting a new climbing location, the possibility of getting lost is very large. That's why we are here for those of you who want to start an adventure</p>
            <NuxtImg 
            src="../public/quote.svg"
            alt="Quote"
            width="186"
            height="219"
            class="camp-quote"
            />
        </div>
    </div>
  </section>
</template>

<script setup lang="ts"></script>

<style scoped></style>
