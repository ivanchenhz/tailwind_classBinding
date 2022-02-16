<script setup>
const switches = [{
  on: true,
}, {
  on: false,
}]
</script>

<template>
  <div class="mt-32 space-y-16">
    <div class="flex items-center justify-around">
      <div
        v-for="s of switches"
        class="w-32 h-32 border-2 border-dashed"
        :class="{ 'bg-pink-300': s.on, 'bg-cyan-300': !s.on }"
      ></div>
    </div>

    <div class="flex items-center justify-around">
      <div
        v-for="s of switches"
        class="w-32 h-32 border-2 border-dashed"
        :class="{ 'bg-pink-300': s.on, 'bg-pink-300': !s.on }"
      ></div>
    </div>
  </div>
</template>
