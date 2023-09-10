<template>
  <section class="flex flex-col justify-center flex-wrap content-center">
    <h1 class="md:text-5xl text-3xl font-extrabold bg-gray-800 text-white w-fit">About Me</h1>
    <div class="lg:w-2/4 text-center m-10">
      <p class="md:text-2xl text-sm font-semibold">{{ about }}</p>
    </div>
  </section>
</template>

<script>
  export default {
    data() {
      return {
        about: `Hi, I am a developer base on cianjur, i recently learn framework frontend nuxt js.
                have experience in backend using express and hapi js also mysql and postgres
                on the database side, still very active learning but I hope I can contribute if given
                the opportunity to join the team, visit my github to find out what I created and let's
                connect`,
      }
    }
  }
</script>