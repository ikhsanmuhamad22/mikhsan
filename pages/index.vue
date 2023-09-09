<template>
  <section class="me flex md:flex-row flex-col flex-wrap justify-center content-center gap-10">
    <div class="me-image md:w-96 w-56">
      <img class="rounded-full shadow-2xl shadow-gray-400" src="../assets/me.jpg" alt="me">
    </div>
    <div class="me-desc flex flex-col flex-wrap justify-center text-center md:w-4/12 md:text-start">
      <p >Hi. {{ me.name }} here</p>
      <p class="md:text-5xl text-3xl font-extrabold">And i'm</p>
      <div class="flex">
        <h1 class="md:text-4xl text-2xl" ref="title">{{ me.title }}</h1>
      </div>
    </div>
  </section>
</template>

<script>
import Typed from 'typed.js';

  export default {
    data() {
      return {
        me: {
          name: 'Ihsan',
          title: '',
        }
      }
    },
    mounted() {
      this.initializeTyped();
    },
    methods: {
      initializeTyped() {
        const options = {
          strings: ['Junior Developer','Web Developer'], 
          typeSpeed: 100, 
          loop: true,
          backSpeed: 50
        };

        const typed = new Typed(this.$refs.title, options);
      },
    },
  }
</script>

<style>
  .typed-cursor {
    font-size: 2rem;
  }
</style>



