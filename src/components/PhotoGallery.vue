<template>
  <div class="mb-12">
    <h3 class="text-2xl font-semibold text-gray-800 mb-6">Memories Together</h3>
    <div class="grid grid-cols-2 md:grid-cols-3 gap-4">
      <!-- Replace with actual photos -->
      <div v-for="i in 6" :key="i" class="aspect-square bg-gray-200 rounded-lg overflow-hidden flex items-center justify-center">
        <span class="text-gray-400">Photo {{ i }}</span>
      </div>
    </div>
    <p class="mt-4 text-sm text-gray-500 text-center">*Replace these placeholders with actual photos*</p>
  </div>
</template>

<script>
export default {
  name: 'PhotoGallery'
}
</script>