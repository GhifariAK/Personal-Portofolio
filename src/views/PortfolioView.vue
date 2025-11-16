PORTOFOLIO VIEW

<script>

export default {
  data() {
    return {
      activeTab: 1,
      items: [
        {
          id: 1,
          name: 'Personal Website',
          imageUrl: 'PersonalPortofolio',
          status: 'My self-developed portfolio website that highlights my professional profile, technical expertise, and project portfolio. This digital space also functions as my technical playground for experimenting with new technologies and development approaches.',
          tech: 'VueJS 3, Tailwind',
          github: 'null',
          demo: 'null',
          notion: 'null'
        },
        {
          id: 2,
          name: 'B-COD Marketplace',
          imageUrl: 'BCOD',
          status: 'B-COD is an exclusive e-commerce marketplace developed specifically for BINUS University academic community. Powered by a Laravel backend and React.js frontend, the platform facilitates secure product transactions among students through an integrated Cash on Delivery (COD) payment solution. The system incorporates robust authentication with student verification, campus-specific delivery zones, and comprehensive order management designed for the university ecosystem.',
          tech: 'Laravel, React.js, MySQL, PHP, JavaScript, Bootstrap, RESTful API',
          github: 'null',
          demo: 'https://b-cod.vercel.app/',
          notion: 'https://www.notion.so/B-COD-1aee6910ef6b80d0baeff3506498d3b2'
        }
      ]
    };
  }
}
</script>
<template>
  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-red-50 mx-3">
    <article data-page="about">
      <header>
        <div
          class="text-2xl font-bold text-white mb-10 fadein-bot title-section flex items-center justify-center flex-col">
          <!-- <div class="h-[1px] w-10 bg-amber-200 md:w-20 aos-init aos-animate"></div> -->
          <h4>Past Project Experience</h4>
          <h4 class="text-base font-normal text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-red-300">
            Discover my portofolio of projects and creative works</h4>
        </div>
      </header>
      <section>
        <div>
          <div class="grid grid-cols-1 gap-4 pb-32 md:grid-cols-3 md:gap-3 xl:grid-cols-3 xl:gap-3 2xl:gap-5 fade-zoom-in">
            <div v-for="item in items" :key="item.id">
              <div
                class="item-card flex flex-col items-center gap-2 rounded bg-[#1e1e1f] hover:bg-[#282828] border border-[#383838] rounded-xl text-amber-50 md:gap-3 px-5 py-5 lg:px-5 ">
                <div class="flex h-12 w-12 items-center justify-center p-0 h-full w-full lg:p-0 zoom-in">
                  <img alt="HTML" loading="lazy" decoding="async" data-nimg="1" class="drop-shadow-xl rounded rounded-xl"
                    :src="'/img/portofolio-' + item.imageUrl + '.png'">
                </div>
                <div class="w-full flex flex-col gap-2 items-center text-sm md:text-base lg:text-lg">
                  <div class="title-text font-medium text-secondary">{{ item.name }}
                  </div>
                  <div class="w-full text-left text-[10px] text-[#c1c1c1] md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                  <div class="w-full mt-4 text-normal text-sm text-left text-red-200">
                    {{ item.tech }}
                  </div>
                  <div class="w-full flex justify-end">
                    <div class="flex cursor-pointer items-end gap-2 text-primary">
                      <a v-if="item.github !== 'null'"
                        :href="item.github" target="_blank" rel="noreferrer"
                        title="View github repository" class="transition-all hover:text-accent">
                        <svg stroke="currentColor"
                          fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                          height="16" width="16" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22">
                          </path>
                        </svg></a>
                        <a v-if="item.demo !== 'null'" :href="item.demo" target="_blank" rel="noreferrer"
                        title="View finished project" class="transition-all hover:text-accent">
                        <svg stroke="currentColor"
                          fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                          height="18" width="18" xmlns="http://www.w3.org/2000/svg">
                          <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
                          <polyline points="15 3 21 3 21 9"></polyline>
                        <line x1="10" y1="14" x2="21" y2="3"></line>
                      </svg></a>
                      <a v-if="item.notion !== 'null'" :href="item.notion" target="_blank" rel="noreferrer"
                        title="View Notion page" class="transition-all hover:text-accent">
                        <!-- Notion logo (monochrome) -->
                        <svg viewBox="0 0 256 256" xmlns="http://www.w3.org/2000/svg" width="18" height="18" fill="currentColor">
                          <path d="M44.2 32.4L149.4 22c10.8-1 19.3 2.1 27.6 8.1l40.5 28.9c6.1 4.4 8.4 9.1 8.4 15.9v133.9c0 12.3-4.7 19.6-18.9 21l-106.2 10.5c-9.1.9-16.8-1.2-25.2-7.2l-44.7-31.6C24.7 195 22 188.9 22 180.5V51.1c0-10.8 7-17.6 22.2-18.7zm12.2 22.7c-5.9.6-7.6 2.6-7.6 7.8v118.6c0 5.4 2.1 7.8 7.4 11l31.8 21.7c3.8 2.6 7.2 3.5 11.1 3.2l94.3-9.3c5.8-.6 7.8-2.9 7.8-8.6V79.2c0-4.7-1.7-7.6-5.8-10.4l-31.1-22c-3.8-2.7-7.2-3.7-11.9-3.2l-96 9.5zM83.4 78.5l54.7-5.4c4.6-.5 7.2 1.1 9.8 4.9l36.5 54.3c1.2 1.8.8 3.2-1.2 3.4l-20.6 2c-4.1.4-6.2-.7-8.6-4l-18.7-27.7-1.1-.1 1.1 33.5c.1 3-.9 4.3-3.7 4.6l-18.2 1.8c-2.8.3-4.1-.8-4.1-3.6l-2.4-60.3c-.1-2.9 1-3.9 3.5-4.2zm-2.1 83.3l91.8-9.1c2.6-.3 3.8.8 4 3.2l1 15.9c.2 2.8-1 4.1-3.6 4.3l-91.9 9.3c-2.6.3-3.9-.9-4.1-3.4l-1.1-16.3c-.2-2.5.9-3.7 3.9-3.9z"/>
                        </svg>
                      </a>
                    </div>
                  </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </article>
</div></template>

<style>
.item-card:hover {
  transition: transform 0.3s ease;
  transform: translateY(-8px);
}
svg:hover{
  stroke: #ffdb70;
}
@keyframes fadeZoomIn {
  0% {
    opacity: 0;
    transform: scale(0.5);
  }
  100% {
    opacity: 1;
    transform: scale(1);
  }
}

/* Menggunakan animasi pada elemen yang diinginkan */
.fade-zoom-in {
  animation: fadeZoomIn 1s ease-in-out;
}
</style>