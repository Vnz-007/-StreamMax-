<template>
  <section
    class="relative w-full h-screen overflow-hidden flex items-center justify-center"
  >
    <div
      id="background__container"
      class="absolute inset-0 h-screen bg-cover bg-no-repeat bg-center -z-10"
    ></div>
    <div
      class="max-w-7xl flex items-center justify-center flex-col mx-auto px-4 sm:px-6 lg:px-8 pt-16"
    >
      <div class="w-full flex items-center space-x-2 mb-4">
        <span
          id="class-mg"
          class="text-white text-sm font-semibold bg-red-600 rounded-full px-3 py-1"
          >SÉRIE ORIGINAL</span
        >
        <div class="flex items-center space-x-1">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="lucide lucide-star w-4 h-4 fill-current text-yellow-400"
          >
            <polygon
              points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"
            ></polygon>
          </svg>
          <span class="text-white text-sm font-medium">8.9</span>
        </div>
      </div>

      <h1
        class="w-full flex flex-col items-start text-4xl sm:text-5xl lg:text-6xl font-bold text-white mb-4 leading-tight"
      >
        Cyberpunk:
        <br />
        <span
          class="text-transparent bg-clip-text bg-gradient-to-r from-red-500 to-orange-500 pb-3"
          >Edgerunners</span
        >
      </h1>
      <p
        id="container-p"
        class="max-w-xl text-left text-gray-300 text-lg sm:text-xl mb-6 leading-relaxed"
      >
        Em uma cidade distópica do futuro, um garoto das ruas tenta sobreviver
        em um mundo onde a tecnologia cibernética e a modificação corporal são a
        norma.
      </p>

      <div
        id="container-class"
        class="w-full flex items-center text-gray-300 space-x-6 mb-8"
      >
        <span class="text-green-500 font-semibold">2025</span>
        <span>10 episódios</span>
        <span>Ação, Ficção Científica, Anime</span>
        <span id="old-class-mg" class="border border-gray-600 text-xs py-1 px-2"
          >16+</span
        >
      </div>

      <div
        class="w-full flex flex-col sm:flex-row items-center justify-start space-y-3 sm:space-y-0 sm:space-x-4 gap-4"
      >
        <button
          class="flex items-center justify-center text-white font-semibold cursor-pointer bg-red-600 hover:bg-red-700 transition-colors rounded-lg space-x-2 shadow-lg py-3 px-12 sm:px-8"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="lucide lucide-play w-5 h-5 fill-current"
          >
            <polygon points="5 3 19 12 5 21 5 3"></polygon>
          </svg>
          <span>Assistir Agora</span>
        </button>

        <button
          class="flex items-center justify-center bg-gray-800/80 hover:bg-gray-700 text-white gap-2 px-8 py-3 rounded-lg font-semibold space-x-2 transition-colors border border-gray-600"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="lucide lucide-info w-5 h-5"
          >
            <circle cx="12" cy="12" r="10"></circle>
            <path d="M12 16v-4"></path>
            <path d="M12 8h.01"></path>
          </svg>
          Mais Informações
        </button>
      </div>
    </div>

    <div
      class="absolute bottom-8 left-1/2 transform -translate-x-1/2 animate-bounce"
    >
      <div
        class="w-6 h-10 border-2 border-white/30 rounded-full flex justify-center"
      >
        <div
          class="w-1 h-3 hidden sm:relative bg-white/60 rounded-full mt-2 animate-pulse"
        ></div>
      </div>
    </div>
  </section>
</template>

<script></script>

<style scoped>
#background__container {
  background: url("../assets/bg-home-desktop.jpg") no-repeat center/cover;
}

.bg-clip-text {
  background-image: linear-gradient(
    to right,
    oklch(63.7% 0.237 25.331),
    oklch(70.5% 0.213 47.604)
  );
  background-clip: text;
  color: transparent;
}
</style>
