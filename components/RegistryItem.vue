<template>
    <div class="registry-item" :class="{ 'purchased': item.purchased }">
      <h3>{{ item.name }}</h3>
      <p>{{ item.description }}</p>
      <a :href="item.link" target="_blank">View Item</a>
      <button @click="togglePurchased" :disabled="item.purchased">
        {{ item.purchased ? 'Purchased' : 'Mark as Purchased' }}
      </button>
    </div>
  </template>
  
  <script setup>
  const props = defineProps(['item'])
  const emit = defineEmits(['update:purchased'])
  
  const togglePurchased = () => {
    emit('update:purchased', props.item.id)
  }
  </script>
  
  <style scoped>
  .registry-item {
    border: 1px solid #ccc;
    padding: 15px;
    margin-bottom: 15px;
  }
  .purchased {
    opacity: 0.5;
  }
  </style>