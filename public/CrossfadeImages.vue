<!-- components/CrossfadeImages.vue -->
<script setup>
import { computed } from 'vue'

const props = defineProps({
  images: { type: Array, required: true },
  scale: { type: Number, default: 1 }, // Add scale prop with default of 1
})

const clicks = computed(() => $slidev.nav.clicks)

// Ensure no extra clicks beyond the last image
const currentImage = computed(() => Math.min(clicks.value, props.images.length - 1))

// Compute the scaling transform style
const scaleStyle = computed(() => ({
  transform: `scale(${props.scale})`
}))
</script>

<template>
  <div class="relative w-full h-full">
    <!-- Add one less click increment to match the number of transitions -->
    <v-click v-for="(_, idx) in images.slice(1)" :key="idx">
      <div />
    </v-click>

    <img
      v-for="(src, idx) in images"
      :key="src"
      :src="src"
      class="absolute inset-0 m-auto max-w-full max-h-full object-contain transition-opacity duration-1"
      :class="currentImage === idx ? 'opacity-100' : 'opacity-0'"
      :style="scaleStyle"
    />
  </div>
</template>
