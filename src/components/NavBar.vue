<template>
  <header
    class="fixed w-full border-b border-gray-800 bg-black/90 backdrop-blur-md z-10"
  >
    <div
      class="max-w-7xl h-16 flex items-center justify-center sm:justify-between lg:justify-center space-x-2 sm:space-x-0 sm:gap-8 mx-auto px-8 sm:px-6 lg:px-8"
    >
      <div>
        <a href="#" class="flex items-center justify-center space-x-2">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="32"
            height="32"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="lucide lucide-play text-red-600 fill-current"
          >
            <polygon points="5 3 19 12 5 21 5 3" />
          </svg>

          <span class="text-white hidden sm:flex text-2xl font-bold">
            Stream
            <span class="text-red-600 text-2xl font-bold back">Max</span>
          </span>
        </a>
      </div>

      <nav>
        <ul
          class="hidden md:flex items-center justify-center space-x-10 lg:space-x-8"
        >
          <li>
            <a
              href="#"
              class="text-gray-300 hover:text-red-500 transition-colors font-medium"
              >Home</a
            >
          </li>
          <li>
            <a
              href="#"
              class="text-gray-300 hover:text-red-500 transition-colors font-medium"
              >Movies</a
            >
          </li>
          <li>
            <a
              href="#"
              class="text-gray-300 hover:text-red-500 transition-colors font-medium"
              >Series</a
            >
          </li>
          <li>
            <a
              href="#"
              class="text-gray-300 hover:text-red-500 transition-colors font-medium"
              >Animes</a
            >
          </li>
          <li>
            <a
              href="#"
              class="text-gray-300 hover:text-red-500 transition-colors font-medium"
              >My list</a
            >
          </li>
        </ul>
      </nav>

      <div
        id="input__container"
        class="max-w-sm hidden lg:flex items-center flex-1 mx-8"
      >
        <div class="w-full relative">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="16"
            height="16"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="lucide lucide-search md:w-5 md:h-5 absolute left-3 top-1/4 transform text-gray-400"
          >
            <circle cx="11" cy="11" r="8" />
            <line x1="21" y1="21" x2="16.65" y2="16.65" />
          </svg>
          <input
            id="search"
            type="text"
            placeholder="Search movies, series, animes..."
            class="w-full text-white border border-gray-700 bg-gray-800 rounded-lg py-2 pl-10 pr-4 outline-none focus:border-red-500 focus:ring-red-500 transition-colors"
          />
        </div>
      </div>

      <div class="flex items-center justify-center space-x-5 lg:space-x-8">
        <a href="#">
          <button
            id="responsive__search-icon"
            class="p-2 cursor-pointer sm:flex lg:hidden"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="lucide lucide-search md:w-5 md:h-5 text-gray-300 hover:text-white transition-colors"
            >
              <circle cx="11" cy="11" r="8" />
              <line x1="21" y1="21" x2="16.65" y2="16.65" />
            </svg>
          </button>
        </a>

        <a href="#">
          <button class="flex items-center justify-center p-2 cursor-pointer">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              fill="#none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="lucide lucide-bell md:w-5 md:h-5 text-gray-300 hover:text-white transition-colors"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <path d="M6 8a6 6 0 0 1 12 0c0 7 3 9 3 9H3s3-2 3-9" />
              <path d="M10.3 21a1.94 1.94 0 0 0 3.4 0" />
            </svg>
          </button>
        </a>

        <a href="#">
          <button class="flex items-center justify-center p-2 cursor-pointer">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="lucide lucide-heart md:w-5 md:h-5 text-gray-300 hover:text-white transition-colors"
            >
              <path
                d="M19 14c1.49-1.46 3-3.21 3-5.5A5.5 5.5 0 0 0 16.5 3c-1.76 0-3 .5-4.5 2-1.5-1.5-2.74-2-4.5-2A5.5 5.5 0 0 0 2 8.5c0 2.3 1.5 4.05 3 5.5l7 7Z"
              />
            </svg>
          </button>
        </a>

        <a href="#">
          <button class="flex items-center justify-center p-2 cursor-pointer">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="lucide lucide-user md:w-5 md:h-5 text-gray-300 hover:text-white transition-colors"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M19 21v-2a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v2"
              />
              <circle cx="12" cy="7" r="4"></circle>
            </svg>
          </button>
        </a>

        <button
          class="flex items-center justify-center p-2 cursor-pointer sm:flex md:hidden"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="32"
            height="32"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="lucide lucide-menu md:w-5 md:h-5 text-gray-300 hover:text-white transition-colors"
          >
            <line x1="4" x2="20" y1="12" y2="12"></line>
            <line x1="4" x2="20" y1="6" y2="6"></line>
            <line x1="4" x2="20" y1="18" y2="18"></line>
          </svg>
        </button>
      </div>
    </div>
  </header>
</template>

<script></script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  font-family: var(--System-UI);
}
</style>
