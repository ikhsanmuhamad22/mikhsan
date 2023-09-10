<template>
  <section class="lg:py-32 lg:px-20 pt-20 h-auto">
    <div class="flex lg:flex-row flex-col justify-center gap-20">
      <div id="mySkill" class="text-center flex-1">
        <h1 class="md:text-3xl text-xl font-extrabold bg-gray-800 text-white w-fit">My Skill</h1>
        <div class="grid lg:grid-cols-5 grid-cols-4 gap-6 lg:m-10 m-3">
          <div v-for="(skill, index) in mySkill" :key="index" class="shadow-md p-4 text-center">
            <img class="md:w-14 w-10" :src="require(`@/assets/icons/${skill.logo}`)" :alt="skill.name">
          </div>
        </div>
      </div>
      <div class="flex flex-col flex-1">
        <h1 class="md:text-3xl text-xl font-extrabold bg-gray-800 text-white w-fit">contact</h1>
        <div class="flex-col shadow-2xl lg:p-10 p-2 lg:m-10 m-3 rounded-lg">
          <div v-for="(item, index) in contact" :key="index" id="contact" class="flex flex-col gap-7">
            <div class="flex flex-row gap-5">
              <div class="p-2 w-14">
                <img :src="require(`@/assets/contact-icons/${item.logo}`)" :alt="item.name">
                </div>
                <a :href="item.link">
                <div class="hover:bg-gray-800 hover:text-white w-fit my-1">
                  <h1 class="text-lg">{{ item.name }}</h1>
                  <p class="text-sm">{{ item.me }}</p>
                </div>
              </a>
              </div>
        </div>
      </div>
    </div>
    </div>
  </section>
</template>

<script>
  export default {
    data() {
      return {
        contact: {

        },
        mySkill: [
          {
          name: 'Html 5',
          logo: 'html.png'
          }, 
          {
          name: 'Css 3',
          logo: 'css-3.png'
          },
          {
          name: 'Bootsrtap',
          logo: 'bootstrap.png'
          },
          {
          name: 'Tailwind',
          logo: 'tailwind.png'
          },
          {
          name: 'Express js',
          logo: 'expressjs.png'
          },
          {
          name: 'Hapijs',
          logo: 'hapijs.png'
          },
          {
          name: 'Sequelize',
          logo: 'Sequelize.png'
          },
          {
          name: 'JavaScript',
          logo: 'js.png'
          },
          {
          name: 'TypeScript',
          logo: 'typescript.png'
          },
          {
          name: 'MySql',
          logo: 'mysql.png'
          },
          {
          name: 'Postgres',
          logo: 'postgre.png'
          },
        ],
        contact: [
          {
          name: 'Email',
          me: 'ikhsanmuhamad3885@gmail.com',
          link: 'mailto:ikhsanmuhamad3885@gmail.com',
          logo: 'gmail.png'
          }, 
          {
          name: 'Facebook',
          me: 'ikhsan muhamad',
          link: 'https://www.facebook.com/profile.php?id=100030205103008',
          logo: 'facebook.png'
          }, 
          {
          name: 'Github',
          me: 'ikhsanmuhamad22',
          link: 'https://github.com/ikhsanmuhamad22',
          logo: 'github.png'
          }, 
          {
          name: 'Linkedin',
          me: 'ihsan muhamad',
          link: 'https://www.linkedin.com/in/ihsan-muhamad-a15698242/',
          logo: 'linkedin-logo.png'
          }, 
          {
          name: 'Instagram',
          me: 'ikhsnmhmd_01',
          link: 'https://www.instagram.com/ikhsnmhmd001_/',
          logo: 'instagram.png'
          }, 
        ]
      }
    }
  }
</script>