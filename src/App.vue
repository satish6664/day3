<script setup>
import ChiLd from '@/components/ChiLd.vue'
import { ref } from 'vue'

const msg = ref('Sai Venkat ')
const msg1 = ref('Pilla')


</script>

<template>
  <h1>{{ msg }} {{ msg1 }}</h1>
  <ChiLd 
    v-model:value="msg" 
    v-model:value1="msg1"
    />
</template>
