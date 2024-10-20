<script setup>
import { RouterLink, RouterView } from 'vue-router'
import TopBarComponent from '@/views/components/TopBarComponent.vue'
import SidebarLibaryComponent from '@/views/components/SidebarLibaryComponent.vue'
</script>

<template>
  <div class="fullscreen-border">
    <TopBarComponent />
    <div class="grid">
      <div class="grid-item">
        <SidebarLibaryComponent />
      </div>
      <div class="grid-item">
        <RouterView />
      </div>
    </div>
  </div>
</template>

<style scoped>
.fullscreen-border {
  padding: 0px 10px;
  background-color: #000000;
}

.grid {
  display: grid;
  grid-template-columns: 300px 1fr;
  gap: 10px;
}

.grid-item {
  background-color: #121212;
  height: 500px;


}

</style>
