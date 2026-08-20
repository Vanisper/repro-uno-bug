<script setup lang="ts">
const female = ref(false)
function switchMale() {
  female.value = !female.value
}
</script>

<template>
  <view @click="switchMale()">
    <text v-if="!female" class="i-material-symbols-male-rounded text-[rgb(0,145,255)]">
      👨 男
    </text>
    <text v-else class="i-material-symbols-female-rounded text-[rgb(255,55,95)]">
      👩 女
    </text>
  </view>
</template>
