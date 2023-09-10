<template>
  <nav class="flex w-screen justify-between p-6 lg:shadow-xl fixed">
    <h1 class="text-xl">Mikhsan</h1>
    <div class="w-auto">
      <div id="list" @click="showNav = !showNav" class="lg:hidden text-end">
        <button v-if="showNav" class="text-gray-800 focus:outline-none">
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
            </svg>
        </button>
        <button v-else  class="text-gray-800 focus:outline-none">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
            </svg>
        </button>
      </div>
      <ul class="lg:flex lg:flex-row flex-col gap-5 font-semibold lg:border-0 border-2 border-black p-5 lg:p-0"
          :class="{ hidden: showNav }">
        <li><nuxt-link to="/">Me.</nuxt-link></li>
        <li><nuxt-link to="/about">About</nuxt-link></li>
        <li><nuxt-link to="/project">Project</nuxt-link></li>
        <li><nuxt-link to="/more">More</nuxt-link></li>
      </ul>
    </div>
  </nav>
</template>

<script>
  export default {
    data() {
      return {
        showNav: true
      }
    }
  }
</script>

