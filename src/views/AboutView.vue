<script>
export default {
  data() {
    return {
      activeTab: 1,
      tech: [
      {
          id: 1,
          name: 'HTML',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/1051/1051277.png',
          status: 'Advanced'
        },
        {
          id: 2,
          name: 'CSS',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/732/732190.png',
          status: 'Advanced'
        },
        {
          id: 3,
          name: 'Javascript',
          imageUrl: 'https://cdn.icon-icons.com/icons2/2415/PNG/512/javascript_original_logo_icon_146455.png',
          status: 'Beginner'
        },
        {
          id: 4,
          name: 'C',
          imageUrl:'https://cdn-icons-png.flaticon.com/512/6132/6132222.png',
          status: 'Advanced'
        },
        {
          id: 5,
          name: 'Java',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/226/226777.png',
          status: 'Advanced'
        },
        {
          id: 6,
          name: 'Python',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/5968/5968350.png',
          status: 'Advanced'
        },
        {
          id: 7,
          name: 'Springboot',
          imageUrl: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg',
          status: 'Beginner'
        },
      ],
      tools: [
        {
          id: 1,
          name: 'Git',
          imageUrl: 'https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png',
          status: 'Version Control'
        },
        {
          id: 2,
          name: 'GitHub',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/25/25231.png',
          status: 'Git Hosting'
        },
        {
          id: 3,
          name: 'MySQL',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/5968/5968313.png',
          status: 'Database'
        },
      ]
    };
  }
}
</script>
<template>
  <!-- Atas -->
  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="about">
      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          About Me &nbsp;
          <div class="h-[1px] w-32 bg-red-500 md:w-96 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
        </div>
      </header>

      <section
        class="text-sm md:text-lg text-justify flex flex-col gap-4 md:flex-row md:gap-8 md:justify-left md:items-center">
        <div class="flex justify-center relative">
            <span class="circle-anim"></span>
            <img
              id="profileAbout"
              alt="avatar"
              width="300"
              height="300"
              decoding="async"
              class="w-300 h-300 md:w-320 md:h-320 rounded-full border-4 border-red-500 pict"
              :src="require('@/assets/FotoProfile.jpg')"
            >
              <span class="dot dot-tl"></span>
              <span class="dot dot-tr"></span>
              <span class="dot dot-bl"></span>
              <span class="dot dot-br"></span>
        </div>
        <div class="md:w-7/12 md:ml-12">
          <p class="mb-3 md:mb-7 fadein-left fadeins-1">
            &nbsp; &nbsp; &nbsp; &nbsp;Hello I'm Ghifari Adam Kesuma, a Computer Science student at BINUS University and a passionate web developer in
            training. I'm currently learning to become a Fullstack Developer, exploring both front-end and back-end
            technologies to build seamless digital experiences. For me, programming isn’t just about solving problems
            — it’s a creative medium to turn ideas into reality.
          </p>
          <p class="mb-3 fadein-left fadeins-2">
            &nbsp; &nbsp; &nbsp; &nbsp; I strive to create digital solutions that don’t just work, but also deliver meaningful experiences. Whether it’s
            front-end or back-end development, I always aim to write efficient code with a personal touch. If you'd like
            to collaborate or connect, feel free to reach out!
          </p>
        </div>

      </section>

    </article>
  </div>

  <!-- Bawah -->
    <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
      <article data-page="about">
        <header>
          <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
            Skills &nbsp;
            <div class="h-[1px] w-10 bg-red-500 md:w-20 aos-init aos-animate" data-aos="zoom-in-left"
              data-aos-duration="600"></div>
          </div>
            <div>
              <p>Technologies & Tools I’m Familiar With</p> <br>
            </div>
        </header>
        <section>
          <div>
            <ul class="flex flex-wrap text-sm font-medium text-center text-red-500 dark:text-red-400 mb-5">
              <li class="mr-2">
                <button class="inline-block px-4 py-3 rounded-lg hover:text-white"
                  :class="{ 'text-red-1000 bg-red-200 bg-opacity-10': activeTab === 1 }" @click="activeTab = 1">Tech Stack</button>
              </li>
              <li class="mr-2">
                <button class="inline-block px-4 py-3 rounded-lg hover:text-white"
                  :class="{ 'text-red-1000 bg-red-200 bg-opacity-10': activeTab === 2 }" @click="activeTab = 2">Tools</button>
              </li>
            </ul>
          </div>

          <div v-show="activeTab === 1">
            <div class="grid grid-cols-2 gap-6 pb-32 md:grid-cols-3 md:gap-10 xl:grid-cols-4 xl:gap-12 2xl:gap-16">
              <div v-for="item in tech" :key="item.id">
                <div
                  class="item-tech-glass flex flex-col items-center justify-center gap-2 rounded-xl border border-gradient px-4 py-6 bg-gradient-to-br from-[#232526cc] to-[#1c1c1ecc] backdrop-blur-md shadow-xl transition-all duration-300 hover:scale-105 hover:border-red-400 hover:bg-[#232526ee] group"
                >
                  <div class="flex h-14 w-14 items-center justify-center mb-2">
                    <img
                      :alt="item.name"
                      loading="lazy"
                      width="40"
                      height="40"
                      decoding="async"
                      class="img-tech drop-shadow-xl transition-all duration-300 group-hover:animate-bounce"
                      :src="item.imageUrl"
                      style="color: transparent;"
                    >
                  </div>
                  <div class="tech font-semibold text-base text-white group-hover:text-[#ff3c3c] transition-all duration-300">{{ item.name }}</div>
                  <div class="status-tech opacity-80 text-xs text-amber-200 mt-1">{{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>

          <div v-show="activeTab === 2">
            <div class="grid grid-cols-2 gap-6 pb-32 md:grid-cols-3 md:gap-10 xl:grid-cols-4 xl:gap-12 2xl:gap-16">
              <div v-for="item in tools" :key="item.id">
                <div
                  class="item-tech-glass flex flex-col items-center justify-center gap-2 rounded-xl border border-gradient px-4 py-6 bg-gradient-to-br from-[#232526cc] to-[#1c1c1ecc] backdrop-blur-md shadow-xl transition-all duration-300 hover:scale-105 hover:border-red-400 hover:bg-[#232526ee] group"
                >
                  <div class="flex h-14 w-14 items-center justify-center mb-2">
                    <img
                      :alt="item.name"
                      loading="lazy"
                      width="40"
                      height="40"
                      decoding="async"
                      class="img-tech drop-shadow-xl transition-all duration-300 group-hover:animate-bounce"
                      :src="item.imageUrl"
                      style="color: transparent;"
                    >
                  </div>
                  <div class="tech font-semibold text-base text-white group-hover:text-[#ff3c3c] transition-all duration-300">{{ item.name }}</div>
                  <div class="status-tech opacity-80 text-xs text-amber-200 mt-1">{{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>

        </section>
      </article>
    </div>
  </template>

<style>
.fadein-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadeins-1 {
  animation-delay: 500ms;
}

.fadeins-2 {
  animation-delay: 800ms;
}

.dot {
  position: absolute;
  border-radius: 50%;
  background: #ff3c3c;
  opacity: 0.8;
  animation: floatCorner 2.5s infinite alternate;
}
.dot-tl { /* Top Left */
  width: 14px; height: 14px;
  top: 0; left: 0;
  animation-delay: 0s;
}
.dot-tr { /* Top Right */
  width: 16px; height: 16px;
  top: 0; right: 0;
  animation-delay: 0.5s;
}
.dot-bl { /* Bottom Left */
  width: 12px; height: 12px;
  bottom: 0; left: 0;
  animation-delay: 1s;
}
.dot-br { /* Bottom Right */
  width: 18px; height: 18px;
  bottom: 0; right: 0;
  animation-delay: 1.5s;
}

@keyframes floatCorner {
  0%   { transform: scale(1) translateY(0);}
  50%  { transform: scale(1.3) translateY(-8px);}
  100% { transform: scale(1) translateY(0);}
}

.circle-anim {
  position: absolute;
  top: 50%; left: 50%;
  transform: translate(-50%, -50%);
  width: 340px; height: 340px;
  border: 3px dashed #ff3c3c;
  border-radius: 50%;
  animation: spinCircle 19s linear infinite;
  z-index: 1;
  opacity: 0.4;
}

@keyframes spinCircle {
  0% { transform: translate(-50%, -50%) rotate(0deg);}
  100% { transform: translate(-50%, -50%) rotate(360deg);}
}

.item-tech-glass {
  border: 2px solid transparent;
  border-image: linear-gradient(90deg, #ff3c3c 0%, #ffe066 100%);
  border-image-slice: 1;
  box-shadow: 0 4px 32px 0 #ff3c3c22;
  background: rgba(30,30,31,0.7);
  transition: box-shadow 0.3s, border 0.3s, background 0.3s;
}
.item-tech-glass:hover {
  box-shadow: 0 8px 40px 0 #ff3c3c55;
  border-color: #ff3c3c;
  background: rgba(30,30,31,0.9);
}
.border-gradient {
  border-image: linear-gradient(90deg, #ff3c3c 0%, #ffe066 100%);
  border-image-slice: 1;
}
.group:hover .img-tech {
  filter: drop-shadow(0 0 8px #ff3c3c);
}
.group:hover .tech {
  color: #ff3c3c;
}
.group:hover .status-tech {
  color: #ffe066;
}

.status-tech {
  color: #ffe066;
  opacity: 0.8;
  text-shadow: 0 1px 4px #ff3c3c33;
}

.group:hover .status-tech {
  color: #ff3c3c; 
}

</style>
