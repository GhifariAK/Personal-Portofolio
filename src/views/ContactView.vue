<template>
  <div class="container mx-auto p-3 md:p-8">
    <div class="flex flex-col items-center justify-center min-h-[70vh]">
      <div class="contact-card-unique relative w-full max-w-3xl bg-[#18181b] rounded-3xl border border-[#ff3c3c] shadow-2xl px-8 py-10 fade-zoom-up">
        <!-- Glow animasi di sudut -->
        <span class="corner-glow glow-tl"></span>
        <span class="corner-glow glow-br"></span>
        <h1 class="text-3xl md:text-4xl font-bold text-white mb-2 text-center tracking-wide">Contact Me</h1>
        <p class="text-base text-slate-300 text-center mb-8">Let's collaborate or just say hi! I love connecting with creative minds.</p>
        
        <!-- Kontak utama -->
        <div class="flex flex-col items-center gap-6 mb-10">
          <div class="contact-circle-card flex flex-col items-center justify-center gap-2 bg-[#1e1e1f] rounded-full border-2 border-[#ff3c3c] px-8 py-6 shadow-lg hover:scale-105 transition-all duration-300">
            <span class="inline-block w-12 h-12 bg-[#ff3c3c] rounded-full flex items-center justify-center animate-pulse">
              <svg width="28" height="28" fill="white"> <path d="M2 4a2 2 0 012-2h20a2 2 0 012 2v20a2 2 0 01-2 2H4a2 2 0 01-2-2V4zm2 0v.01L14 14l8-9.99V4H4zm0 2.41V24h20V6.41l-10 9.99-10-9.99z"/></svg>
            </span>
            <div class="font-semibold text-white mt-2">Personal Email</div>
            <a href="mailto: ghifariadamkesuma@gmail.com" class="text-xs text-slate-300 underline 
            hover:text-[#ff3c3c] transition-colors">ghifariadamkesuma@gmail.com</a>
            
          </div>

          <div class="contact-circle-card flex flex-col items-center justify-center gap-2 bg-[#1e1e1f] rounded-full border-2 border-[#ff3c3c] px-8 py-6 shadow-lg hover:scale-105 transition-all duration-300">
            <span class="inline-block w-12 h-12 bg-[#ff3c3c] rounded-full flex items-center justify-center animate-pulse">
              <svg width="28" height="28" fill="white"> <path d="M2 4a2 2 0 012-2h20a2 2 0 012 2v20a2 2 0 01-2 2H4a2 2 0 01-2-2V4zm2 0v.01L14 14l8-9.99V4H4zm0 2.41V24h20V6.41l-10 9.99-10-9.99z"/></svg>
            </span>
            <div class="font-semibold text-white mt-2">University Email</div>
            <a href="mailto: ghifari.kesuma@binus.ac.id" class="text-xs text-slate-300 underline 
            hover:text-[#ff3c3c] transition-colors">ghifari.kesuma@binus.ac.id</a>
          </div>
        </div>

        <!-- Sosmed lingkaran dengan logo asli -->
        <div class="flex justify-center gap-8 mb-10">
          <!-- LinkedIn -->
          <a href="https://www.linkedin.com/in/ghifari-adam-kesuma-518a151b1/" target="_blank" class="socmed-circle group">
            <span class="inline-block w-12 h-12 bg-[#ff3c3c] rounded-full flex items-center justify-center transition-all duration-300 group-hover:scale-110 group-hover:bg-[#0077b5] animate-pulse">
              <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 24 24" fill="white">
                <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/>
              </svg>
            </span>
          </a>
          
          <!-- GitHub -->
          <a href="https://github.com/GhifariAK" target="_blank" class="socmed-circle group">
            <span class="inline-block w-12 h-12 bg-[#ff3c3c] rounded-full flex items-center justify-center transition-all duration-300 group-hover:scale-110 group-hover:bg-[#333] animate-pulse">
              <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 24 24" fill="white">
                <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
              </svg>
            </span>
          </a>
        </div>

        <!-- CTA unik -->
        <div class="mt-6 text-center">
          <div class="text-lg font-bold text-white mb-2">Let's Build Something Awesome!</div>
          <div class="text-base text-slate-300 mb-4">Open for freelance, collaboration, or just a friendly chat.</div>
          <a href="mailto:ghifariadamkesuma@gmail.com" class="inline-flex items-center gap-2 px-7 py-3 rounded-full bg-[#ff3c3c] text-white font-semibold hover:bg-[#ff5c5c] transition-all duration-300 shadow-lg">
            <svg width="20" height="20" fill="white"><path d="M2 4a2 2 0 012-2h12a2 2 0 012 2v12a2 2 0 01-2 2H4a2 2 0 01-2-2V4zm2 0v.01L10 10l6-5.99V4H4zm0 2.41V18h12V6.41l-6 5.99-6-5.99z"/></svg>
            Send Message
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.contact-card-unique {
  position: relative;
  overflow: hidden;
  background: rgba(30,30,31,0.85);
  backdrop-filter: blur(2px);
}
.corner-glow {
  position: absolute;
  border-radius: 50%;
  pointer-events: none;
  z-index: 0;
  animation: glowAnim 3s infinite alternate;
}
.glow-tl {
  top: -40px; left: -40px;
  width: 120px; height: 120px;
  box-shadow: 0 0 80px 40px #ff3c3c88;
}
.glow-br {
  bottom: -40px; right: -40px;
  width: 120px; height: 120px;
  box-shadow: 0 0 80px 40px #ff3c3c88;
}
@keyframes glowAnim {
  0% { opacity: 0.7; }
  100% { opacity: 1; }
}
.contact-circle-card {
  transition: box-shadow 0.3s, transform 0.3s;
}
.socmed-circle {
  transition: transform 0.3s;
}
.fade-zoom-up {
  animation: fadeZoomUp 1s ease-in-out;
}
@keyframes fadeZoomUp {
  0% { opacity: 0; transform: scale(0.8);}
  100% { opacity: 1; transform: scale(1);}
}
</style>