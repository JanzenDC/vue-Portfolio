<template>
  <main>
    <nav class="px-4 p-8 md:px-14 bg-[#435334] border-b" :class="{'fixed-nav': isNavFixed}">
    <div class="flex justify-between">
      <div class="flex">
              <img src="@/images/jdc_logo.png" alt="Logo" class="w-10 h-10">
              <h1 class="py-2 text-white">Janzen Dela Cruz</h1>
      </div>
      <div class="md:hidden block text-white text-2xl">
        <i class="bi bi-list" @click="toggleMenu"></i>
      </div>
      <div class="md:hidden bg-[#435334] w-full h-full p-4 fixed mt-[69px] " v-show="isMenuOpen">
        <ul>
          <li class="text-[#9EB384] hover:border-b">
            <a @click="scrollToSection('Home')">
              #<span class="text-[#CEDEBD]">Home</span>
            </a>
          </li>
          <li class="text-[#9EB384] hover:border-b">
            <a @click="scrollToSection('Skills')">  
              #<span class="text-[#CEDEBD]">Skills</span>
            </a>
          </li>
          <li class="text-[#9EB384] hover:border-b">
            <a @click="scrollToSection('Works')">
              #<span class="text-[#CEDEBD]">Works</span>
            </a>
          </li>
          <li class="text-[#9EB384] hover:border-b">
            <a @click="scrollToSection('About-me')">
              #<span class="text-[#CEDEBD]">About-me</span>
            </a>
          </li>
        </ul>
        <div class="flex justify-center items-center gap-3 mt-5">
          <div class="items-center flex justify-center text-[#435334] p-3 text-2xl bg-[#CEDEBD] rounded-sm">
            <a href="https://www.linkedin.com/in/janzen-forrest-dela-cruz-a3a988292/"><i class="bi bi-linkedin"></i></a>
          </div>
          <div class="items-center flex justify-center text-[#435334] p-3 text-2xl bg-[#CEDEBD] rounded-sm">
            <a href="https://github.com/JanzenDC"><i class="bi bi-github"></i></a>
          </div>
        </div>
    </div>
      <ul class="md:flex items-center gap-10 hidden">
        <li class="text-[#9EB384] hover:border-b">
          <a @click="scrollToSection('Home')">
            #<span class="text-[#CEDEBD]">Home</span>
          </a>
        </li>
        <li class="text-[#9EB384] hover:border-b">
          <a @click="scrollToSection('Skills')">
            #<span class="text-[#CEDEBD]">Skills</span>
          </a>
        </li>
        <li class="text-[#9EB384] hover:border-b">
          <a @click="scrollToSection('Resume')">
            #<span class="text-[#CEDEBD]">Resume</span>
          </a>
        </li>
        <li class="text-[#9EB384] hover:border-b">
          <a @click="scrollToSection('Works')">
            #<span class="text-[#CEDEBD]">Works</span>
          </a>
        </li>
        <li class="text-[#9EB384] hover:border-b">
          <a @click="scrollToSection('About-me')">
            #<span class="text-[#CEDEBD]">About-me</span>
          </a>
        </li>
      </ul>
    </div>

    <div class="absolute mt-5 hidden md:block">
      <div class="p-3 items-center flex justify-center">
        <div class="bg-[#CEDEBD] h-[50px] w-1"></div>
      </div>
      <div class="items-center flex justify-center text-[#435334] p-3 text-2xl bg-[#CEDEBD] mt-1 rounded-sm">
        <a href="https://www.linkedin.com/in/janzen-forrest-dela-cruz-a3a988292/"><i class="bi bi-linkedin"></i></a>
      </div>
      <div class="items-center flex justify-center text-[#435334] p-3 text-2xl bg-[#CEDEBD] mt-3 rounded-sm">
        <a href="https://github.com/JanzenDC"><i class="bi bi-github"></i></a>
      </div>
    </div>

    </nav>

    <section id="Home" class="p-4 md:px-60 bg-[#435334]">
      <div class="lg:flex ">
        <div class=" w-full ">
          <h1 class="text-4xl text-white font-bold">Janzen is a <span class="text-[#9EB384]">full-stack developer</span> with a profound passion for crafting exquisite and highly responsive websites.</h1>
          <p class="text-1xl text-white mt-2">He creates responsive websites that integrate technology and creativity.</p>
          <div class="p-3 mt-3 px-0">
            <a class="text-1xl text-white p-2 border-white border px-10 hover:bg-[#a8e26b]">Contact Me</a>
          </div>
        </div>
        <div class="mt-10 w-full">
          <div class="w-full flex justify-end items-end">
            <img src="@/images/pixels-neon.gif" alt="Image Description" class="w-full md:w-96">
          </div>
          <div class="flex justify-end items-end ">
            <div class="p-1 flex gap-1 border">
              <div class="bg-green-500 w-3 h-3 items-center justify-center mt-1"></div>
              <p class="text-white">Currently working on Portfolio</p>
            </div>
          </div>
        </div>
      </div>
      <div class="flex justify-center mt-4 ">
        
        <div class="p-10 ">
          <div class="relative flex">
            <img src="@/images/qoutation.png" class="w-10 h-10 absolute -top-4 left-5">
            <div class="p-5 border-[#9EB384] border text-1xl text-white">
              
              Courage has breathed life into countless dreams, while fear has buried them in the depths of doubt
            </div>
            <img src="@/images/qoutation.png" class="w-10 h-10 absolute -bottom-6 right-8">
          </div>
        </div>
      </div>
    </section>

    <section id="Skills" class="p-4 md:px-60 bg-[#435334]">
      <div class="flex">
          <h1 class="text-4xl text-white"><span class="text-[#9EB384]">#</span>Skills</h1>
          <div class="py-4 px-4">
            <div class="bg-white w-64 h-1 md:block hidden"></div>
          </div>
      </div>
      <div class="md:flex w-full">
        <div class="w-1/2">
          <img src="@/images/img-bg.png" alt="Alternate Image" class="w-80">
        </div>
        <div>
          <div class="grid grid-cols-2 md:grid-cols-3 gap-4"> 
            <div class="border">
              <div class="p-2 text-white border-b">
                Languages
              </div>
              <div class="p-2 text-white">
                Javascript, Java, PHP
              </div>
            </div>
            <div class="border">
              <div class="p-2 text-white border-b">
                Databases
              </div>
              <div class="p-2 text-white">
                MySql
              </div>
            </div>
            <div class="border">
              <div class="p-2 text-white border-b">
                Server side
              </div>
              <div class="p-2 text-white">
                Node
              </div>
            </div>
            <div class="border lg:hidden">
              <div class="p-2 text-white border-b">
                Other
              </div>
              <div class="p-2 text-white">
                HTML, CSS, EJS, Vite
              </div>
            </div>               
          </div>

          <div class="grid grid-cols-2 md:grid-cols-3 gap-4 mt-3"> 
            <div class="border ">
              <div class="p-2 text-white border-b">
                Frameworks
              </div>
              <div class="p-2 text-white ">
                Vue, Tailwind, Bootstrap, Quasar
              </div>
            </div>
            <div class="border ">
              <div class="p-2 text-white border-b">
                Tools
              </div>
              <div class="p-2 text-white">
                VSCode, Git, Insomnia, Xampp
              </div>
            </div>
            <div class="order-first md:block hidden">

            </div>
          </div>


          <div class="grid grid-cols-2 md:grid-cols-3 gap-4 mt-3"> 
            <div class="order-first md:block hidden">

            </div>
            <div class="order md:block hidden">

            </div>
            <div class="border hidden lg:block">
              <div class="p-2 text-white border-b">
                Other
              </div>
              <div class="p-2 text-white">
                HTML, CSS, EJS, Vite
              </div>
            </div>           
          </div>
        </div>
      </div>


    </section>

    <section id="Works" class="p-4 md:px-60 bg-[#435334]">
      <div class="flex">
          <h1 class="text-4xl text-white"><span class="text-[#9EB384]">#</span>Projects</h1>
          <div class="py-4 px-4">
            <div class="bg-white w-64 h-1 md:block hidden"></div>
          </div>
      </div>
      <div class="md:flex mt-3 gap-16">
        <div class="md:w-72 w-full">
          <img src="@/images/static_nft_marketplace.png" alt="background logo" class="lg:w-96 w-full">
          <div class="text-white p-4 border">
            Tailwind CSS, Javascript, HTML
          </div>
          <div class="text-white p-4 border h-[180px]">
            <h1 class="font-bold">NFT MARKETPLACE UI</h1>
            <p>A static Web page for NFT</p>
            <div class="flex mt-7 gap-4">
              <div class="gap-1 p-1 border-[#9EB384] border w-20 flex justify-center items-center hover:bg-[#a8e26b]">
                <a href="https://janzendc.github.io/NFT-Marketplace-UI/">Live </a> <i class="bi bi-paperclip rotate-45"></i>
              </div>            
              <div class="gap-1 p-1 border-[#9EB384] border w-20 flex justify-center items-center hover:bg-[#a8e26b]">
                <a href="https://github.com/JanzenDC/NFT-Marketplace-UI">Repo </a> <i class="bi bi-github"></i>
              </div>
              
            </div>
          </div>
        </div>

        <div class="md:w-72  md:mt-0 mt-3 w-full ">
          <img src="@/images/static_password_checker.png" alt="background logo" class="lg:w-96 w-full">
          <div class="text-white p-4 border">
            Bootstrap, Javascript, HTML
          </div>
          <div class="text-white p-4 border h-[180px]">
            <h1 class="font-bold">Simple Password Checker</h1>
            <p>A static Web page checking your password if it is weak or strong</p>
            <div class="flex mt-1 gap-4">
              <div class="gap-1 p-1 border-[#9EB384] border w-20 flex justify-center items-center hover:bg-[#a8e26b]">
                <a href="https://janzendc.github.io/Password-Strength-Checker/">Live </a> <i class="bi bi-paperclip rotate-45"></i>
              </div>            
              <div class="gap-1 p-1 border-[#9EB384] border w-20 flex justify-center items-center hover:bg-[#a8e26b]">
                <a href="https://github.com/JanzenDC/Password-Strength-Checker">Repo </a> <i class="bi bi-github"></i>
              </div>
              
            </div>
          </div>
        </div>
        <div class="md:w-72  md:mt-0 mt-3 w-full ">
          <img src="@/images/static_password_generator.png" alt="background logo" class="lg:w-96 w-full">
          <div class="text-white p-4 border">
            Bootstrap, Javascript, HTML
          </div>
          <div class="text-white p-4 border h-[180px]">
            <h1 class="font-bold">Simple Password Generator</h1>
            <p>A static Web page that can generate strong passwords</p>
            <div class="flex mt-1 gap-4">
              <div class="gap-1 p-1 border-[#9EB384] border w-20 flex justify-center items-center hover:bg-[#a8e26b]">
                <a href="https://janzendc.github.io/Password-Generator/">Live </a> <i class="bi bi-paperclip rotate-45"></i>
              </div>            
              <div class="gap-1 p-1 border-[#9EB384] border w-20 flex justify-center items-center hover:bg-[#a8e26b]">
                <a href="https://github.com/JanzenDC/Password-Generator">Repo </a> <i class="bi bi-github"></i>
              </div>
            </div>
          </div>

          
        </div>
        <div class="md:w-72  md:mt-0 mt-3 w-full ">
          <img src="@/images/New_Project.png" alt="background logo" class="lg:w-96 w-full">
          <div class="text-white p-4 border">
            Tailwind and Vue
          </div>
          <div class="text-white p-4 border h-[200px]">
            <h1 class="font-bold">Commercial Website</h1>
            <p>Commercial Website for WeaveManila</p>
            <div class="flex mt-14 gap-4">
              <div class="gap-1 p-1 border-[#9EB384] border w-20 flex justify-center items-center hover:bg-[#a8e26b]">
                <a href="https://weave-manila-ui.vercel.app/">Live </a> <i class="bi bi-paperclip rotate-45"></i>
              </div>            
              <div class="gap-1 p-1 border-[#9EB384] border w-20 flex justify-center items-center hover:bg-[#a8e26b]">
                <a href="https://github.com/JanzenDC/WeaveManila-Ui">Repo </a> <i class="bi bi-github"></i>
              </div>
              
            </div>
          </div>

          
        </div>
      </div>
    </section>

    <section id="About-me" class="p-4 md:px-60 bg-[#435334]">
      <div class="flex">
          <h1 class="text-4xl text-white "><span class="text-[#9EB384]">#</span>about-me</h1>
          <div class="py-4 px-4">
            <div class="bg-white w-64 h-1 md:block hidden"></div>
          </div>
      </div>
      <div class="md:flex gap-14">
        <div class="text-[#9EB384] md:text-2xl mt-3 text-justify">
          <p>
            <h1>Hello, I am Janzen!</h1>
            <p class="mt-3">
              My journey becoming a self-taught developer began on my 7th Grade with Java and Basic HTML,CSS.
              My passion for coding was continue untill now I am taking BSIT 4th year at Forbes College. I have 
              continued to expand my skills in both Front-End and Back-End development.
            </p>
          </p>
        </div>
        <div class="md:justify-end md:items-end md:flex w-full items-center justify-center">
          <img src="@/images/bg_image_myself.jpg" alt='image of me' class="w-64">
        </div>
      </div>
    </section>

    <section id="Footer" class="p-4 md:px-60 bg-[#435334] border-white border-t">
      <div>
        <div class="justify-between md:flex">

          <div class="flex">
            <img src="@/images/jdc_logo.png" alt="Logo" class="w-10 h-10">
            <p class="p-2 text-white">janzendelacruz28@gmail.com</p>
          </div>

          <div class="p-4 text-white hidden md:block">
            <div>
              <p>Message me here</p>
            </div>
            <div>
              <div class="gap-2 flex text-1xl">
                <i class="bi bi-discord"></i>
                <div>Habibi!</div>
              </div>
              <div class="gap-2 flex text-1xl">
                <i class="bi bi-envelope"></i>
                <div>janzendelacruz28@..</div>
              </div>
            </div>
          </div>

          <div class="p-4 text-white md:hidden">
            <div>
              <p>Message me here</p>
            </div>
            <div>
              <div class="gap-2 flex text-1xl">
                <i class="bi bi-discord"></i>
                <div>Habibi!</div>
              </div>
              <div class="gap-2 flex text-1xl">
                <i class="bi bi-envelope"></i>
                <div>janzendelacruz28@gmail.com</div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="flex justify-center items-center mt-10 text-[#9EB384]">
        © Copyright 2023. Made by Janzen
      </div>
    </section>
  </main>
</template>

<style scoped>
.fixed-nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #435334;
  z-index: 1000;
  /* Add other styling as needed */
}
</style>


<script>
export default {
  data() {
    return {
      isNavFixed: false,
      isMenuOpen: false,
    };
  },
  created() {
    window.addEventListener('scroll', this.handleScroll);
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
    handleScroll() {
      const scrollY = window.scrollY;
      if (scrollY > 0 && !this.isNavFixed) {
        this.isNavFixed = true;
      } else if (scrollY === 0 && this.isNavFixed) {
        this.isNavFixed = false;
      }
    },
    scrollToSection(sectionId) {
      const section = document.getElementById(sectionId);
      if (section) {
        section.scrollIntoView({ behavior: 'smooth' });
        this.isMenuOpen = false; 
      }
    },
  },
};
</script>