<script setup>
import BaseIcon from './BaseIcon.vue';
import { computed, onMounted, ref } from 'vue'
const emit = defineEmits(['timerDone'])
const props = defineProps({
  time: {
    type: String,
  }
})
const timer = ref('')

onMounted(() => {
  // startTimer()
})


</script>

<template>
  <div class="w-54px z-8">
    <BaseIcon
      name="cub"
      :w="54"
      :h="26"
      class="-z-1 pointer-events-none absolute"
    />
    <span class="font-400 text-white text-18px leading-24px w-43px z-10">{{ time }}</span>
  </div>
</template>

<style scoped lang="scss">
</style>


