<template>
  <section
    class="max-container padding-container flex flex-col gap-20 py-10 pb-32 md:gap-28 lg:py-20 xl:flex-row"
  >
    <div class="hero-map" />
    <!-- leftside -->
    <div class="relative z-20 flex-1 flex-col xl:w1/2">
      <NuxtImg
        src="camp.svg"
        alt="Camp"
        width="50"
        height="50"
        class="absolute left-[-5px] top-[-30px] w-10 lg:w-[50px]"
      />
      <h1 class="bold-52 lg:bold-88">Putuk Truno Camp Area</h1>
      <p class="regular-16 mt-6 text-gray-30 xl:max-w-[520px]">
        We want to be on each of your journeys seeking the satisfaction of
        seeing the incorruptible beauty of nature. We can help you on an
        adventure around the world in just one app
      </p>
      <div class="my-11 flex flex-wrap gap-5">
        <div class="flex items-center gap-2">
          <NuxtImg
            v-for="n in 5"
            src="star.svg"
            alt="Star"
            width="24"
            height="24"
          />
        </div>
        <p class="bold-16 lg:bold-20 text-blue-70">
          198k
          <span class="regular-16 lg:regular-20 ml-1">Excellent Reviews</span>
        </p>
      </div>
      <div class="flex flex-col w-full gap-3 sm:flex-row">
        <TheButton type="button" title="Download App" variant="btn_green" />
        <TheButton
          type="button"
          title="How We Work?"
          icon="../public/play.svg"
          variant="btn_white_text"
        />
      </div>
    </div>

    <div class="relative flex flex-1 items-start">
      <div
        class="relative z-20 flex w-[268px] flex-col gap-8 rounded-3xl bg-green-90 px-7 py-8"
      >
        <div class="flex flex-col">
          <div class="flexBetween">
            <p class="regular-16 text-gray-20">Location</p>
            <NuxtImg
              src="close.svg"
              alt="Close"
              width="24"
              height="24"
            />
          </div>
          <p class="bold-20 text-white">Aguas Calientes</p>
        </div>

        <div class="flexBetween">
          <div class="flex flex-col">
            <p class="regular-16 text-gray-20">Distance</p>
            <p class="bold-20 text-white">173.28 mi</p>
          </div>
          <div class="flex flex-col">
            <p class="regular-16 text-gray-20">Elevation</p>
            <p class="bold-20 text-white">5.020 km</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts"></script>

<style scoped></style>
