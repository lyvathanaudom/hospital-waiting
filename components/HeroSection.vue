<!-- components/HeroSection.vue -->
<template>
  <section class="py-6">
    <div
      class="flex flex-col-reverse md:flex-row items-center justify-between gap-8"
    >
      <div class="md:w-1/2 text-center md:text-left">
        <h1 class="sm:text-4xl text-2xl font-bold text-gray-800 mb-4">
          Hospital Waiting Period
        </h1>
        <p class="text-gray-600 mb-6">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed eget
          libero feugiat.
        </p>
        <Button text="Learn More" />
      </div>
      <Illustration class="sm:w-5/12" />
    </div>
  </section>
</template>