<script setup>

</script>

<template>
  <div class="bg-fuchsia-50 p-8">
    <h1 class="mb-4">projects</h1>
    <p class="mb-8 nunito">Some of the projects that I have worked on</p>
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4 nunito">
      <!-- Wasabi photo -->
      <div class="bg-white p-4 mb-4 hover:translate-y-7 hover:border-4 hover:border-pink-100">
        <h2 class="text-xl mb-2">Wasabi dataviz</h2>
        <img src="./../assets/Wasabi_dataviz.png" alt="Wasabi image" class="w-104 h-104 md:w-112 lg:w-120 xl:w-112 lg:h-120 xl:h-120 object-cover mb-4 md:mb-0">
      </div>

      <!-- MiageLand -->
      <div class="bg-white p-4 mb-4 hover:border-4 hover:border-pink-100 hover:translate-y-7">
        <h2 class="text-xl mb-2">MIAGE Land</h2>
        <img src="./../assets/miageLand.png" alt="Miage Land image" class="w-104 h-104 md:w-112 lg:w-120 xl:w-112 lg:h-120 xl:h-120 object-cover mb-4 md:mb-0">
      </div>

      <!-- Portfolio -->
      <div class="bg-white p-4 mb-4 hover:border-4 hover:border-pink-100 hover:translate-y-7">
        <h2 class="text-xl mb-2">Portfolio</h2>
        <img src="./../assets/portfolio.png" alt="Portfolio image" class="w-104 h-104 md:w-112 lg:w-120 xl:w-112 lg:h-120 xl:h-120 object-cover mb-4 md:mb-0">
      </div>

      <!-- Wasabi description -->
      <div class="wasabi-description-container bg-pink-100 p-4 mb-4">
        <p class="text-balance text-center">A university project involving data visualization,
          using a music API. The data processing is accomplished using <span class="underline text-pink-800 font-bold">Python</span>,
          the frontend is developed in <span class="underline text-pink-800 font-bold">Vue.js</span>, and the graphs are implemented using
          <span class="underline text-pink-800 font-bold">D3.js</span></p>
      </div>

      <!-- MiageLand description-->
      <div class="bg-pink-100  p-4 mb-4">
        <p class="text-balance text-center">A university project focusing on the development
          of an amusement park management application has been implemented using <span class="underline text-pink-800 font-bold">Spring Boot</span>
          for the backend and <span class="underline text-pink-800 font-bold">Vue.js</span> for the frontend.
        </p>
      </div>

      <!-- Portfolio description -->
      <div class="bg-pink-100  p-4 mb-4">
        <p class="text-balance text-center">Personal project to get better at using <span class="underline text-pink-800 font-bold">Vue.js</span>.</p>
      </div>
    </div>



  </div>
</template>

<style scoped>
  /* Styles for Wasabi photo */


/* Styles for Wasabi description */
.wasabi-description-container {
  border: 2px solid transparent; /* Bordure initiale */
  transition: border-color 0.3s ease; /* Ajouter une transition pour une animation fluide */
  /* Autres styles... */
}

/* Styles pour changer la bordure lorsqu'on survole Wasabi photo */
.wasabi-photo-container:hover .wasabi-description-container {
  border-color: #ff4081; /* Changer la couleur de la bordure au survol */
}
</style>