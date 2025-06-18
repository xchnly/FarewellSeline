<template>
  <div class="mb-12">
    <h3 class="text-2xl font-semibold text-gray-800 mb-6 text-center relative">
      <span class="relative z-10 px-4 bg-white">Memories Together</span>
      <div class="absolute top-1/2 left-0 right-0 h-px bg-gray-200 z-0"></div>
    </h3>
    
    <div class="grid grid-cols-2 md:grid-cols-3 gap-4">
      <div v-for="i in 6" :key="i" class="aspect-square bg-gradient-to-br from-pink-50 to-purple-50 rounded-lg overflow-hidden flex items-center justify-center relative group">
        <div class="absolute inset-0 flex items-center justify-center opacity-20">
          <svg class="w-16 h-16 text-pink-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M12.395 2.553a1 1 0 00-1.45-.385c-.345.23-.614.558-.822.88-.214.33-.403.713-.57 1.116-.334.804-.614 1.768-.84 2.734a31.365 31.365 0 00-.613 3.58 2.64 2.64 0 01-.945-1.067c-.328-.68-.398-1.534-.398-2.654A1 1 0 005.05 6.05 6.981 6.981 0 003 11a7 7 0 1011.95-4.95c-.592-.591-.98-.985-1.348-1.467-.363-.476-.724-1.063-1.207-2.03zM12.12 15.12A3 3 0 017 13s.879.5 2.5.5c0-1 .5-4 1.25-4.5.5 1 .786 1.293 1.371 1.879A2.99 2.99 0 0113 13a2.99 2.99 0 01-.879 2.121z" clip-rule="evenodd"></path></svg>
        </div>
        <span class="text-gray-400 z-10">Photo {{ i }}</span>
        <div class="absolute bottom-2 right-2 w-8 h-8 bg-pink-500 text-white rounded-full flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity">
          <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 8V4m0 0h4M4 4l5 5m11-1V4m0 0h-4m4 0l-5 5M4 16v4m0 0h4m-4 0l5-5m11 5l-5-5m5 5v-4m0 4h-4"></path></svg>
        </div>
      </div>
    </div>
    <p class="mt-4 text-sm text-gray-500 text-center">*Replace these placeholders with actual photos*</p>
  </div>
</template>