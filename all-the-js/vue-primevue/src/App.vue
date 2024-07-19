<script setup lang="ts">
import { $dt } from "@primevue/themes";

const menuBarTextColor = $dt("emerald.500").value;
</script>

<template>
  <Menubar>
    <template #start>
      <div :style="`color: ${menuBarTextColor};`" class="flex items-center">
        <div style="text-align: center" class="mr-2">vue - primevue -</div>
        <div><i class="pi pi-prime" style="font-size: 1.5rem"></i></div>
      </div>
    </template>
  </Menubar>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
