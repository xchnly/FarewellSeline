<template>
  <div class="min-h-screen bg-gradient-to-b from-blue-50 to-purple-50 py-12 px-4 sm:px-6 lg:px-8">
    <div class="max-w-3xl mx-auto">
      <!-- Header -->
      <div class="text-center mb-12">
        <h1 class="text-4xl font-extrabold text-gray-900 sm:text-5xl sm:tracking-tight lg:text-6xl">
          Farewell Seline
        </h1>
        <p class="mt-5 max-w-xl mx-auto text-xl text-gray-500">
          Wishing you all the best in your new journey!
        </p>
      </div>

      <!-- Main Content -->
      <div class="bg-white shadow-xl rounded-lg overflow-hidden">
        <!-- Hero Section -->
        <div class="bg-blue-600 p-8 text-white text-center">
          <h2 class="text-3xl font-bold mb-4">Shipping Department</h2>
          <p class="text-xl opacity-90">Thank you for your dedication and hard work!</p>
        </div>

        <!-- Components -->
        <div class="p-8">
          <FarewellMessage />
          <PhotoGallery />
          
          <!-- Team Signatures -->
          <div class="mt-12 border-t pt-8">
            <h3 class="text-2xl font-semibold text-gray-800 mb-6">From Your Team</h3>
            <div class="grid grid-cols-2 sm:grid-cols-3 gap-4">
              <div v-for="(member, index) in teamMembers" :key="index" class="text-center">
                <div class="h-16 w-16 mx-auto bg-blue-100 rounded-full flex items-center justify-center text-blue-600 font-bold text-xl mb-2">
                  {{ member.initials }}
                </div>
                <p class="font-medium">{{ member.name }}</p>
                <p class="text-sm text-gray-500">{{ member.position }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Footer -->
      <div class="mt-12 text-center text-gray-500 text-sm">
        <p>Created with ❤️ by 出库管理群 - 出库 PMC 船务</p>
        <p class="mt-1">{{ currentDate }}</p>
      </div>
    </div>
  </div>
</template>

<script>
import FarewellMessage from './components/FarewellMessage.vue'
import PhotoGallery from './components/PhotoGallery.vue'

export default {
  components: {
    FarewellMessage,
    PhotoGallery
  },
  data() {
    return {
      currentDate: new Date().toLocaleDateString('en-US', { 
        year: 'numeric', 
        month: 'long', 
        day: 'numeric' 
      }),
      teamMembers: [
        { name: '恒利', initials: 'HL', position: 'PMC' },
        { name: '进龙', initials: 'JL', position: '仓库' },
        { name: '豪俊', initials: 'HJ', position: 'PMC' },
        { name: '芳芳', initials: 'FF', position: 'PMC' },
        { name: '资阳', initials: 'ZY', position: '船务' },
        { name: 'Arthur', initials: 'AR', position: '船务' },
      ]
    }
  }
}
</script>