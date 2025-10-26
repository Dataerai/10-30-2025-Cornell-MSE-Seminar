<template>
  <div 
    :class="[
      'absolute z-10',
      position === 'top' ? 'top-5' : 'bottom-5',
      align === 'left' ? 'left-5' : align === 'right' ? 'right-5' : 'left-1/2 transform -translate-x-1/2',
      customClass
    ]"
    :style="{
      fontSize: fontSize || '12px',
      color: color || '#666',
      fontWeight: fontWeight || 'normal',
      ...customStyle
    }"
  >
    <a 
      v-if="href && href !== '#'" 
      :href="href" 
      target="_blank" 
      rel="noopener noreferrer"
      class="hover:underline"
    >
      {{ reference }}
    </a>
    <span v-else>
      {{ reference }}
    </span>
  </div>
</template>

<script setup>
defineProps({
  href: {
    type: String,
    default: ''
  },
  reference: {
    type: String,
    required: true
  },
  position: {
    type: String,
    default: 'bottom',
    validator: (value) => ['top', 'bottom'].includes(value)
  },
  align: {
    type: String,
    default: 'left',
    validator: (value) => ['left', 'right', 'center'].includes(value)
  },
  offset: {
    type: String,
    default: '20px'
  },
  fontSize: {
    type: String,
    default: '12px'
  },
  fontWeight: {
    type: String,
    default: 'normal'
  },
  color: {
    type: String,
    default: '#666'
  },
  class: {
    type: String,
    default: ''
  },
  customClass: {
    type: String,
    default: ''
  },
  customStyle: {
    type: Object,
    default: () => ({})
  }
})
</script>
