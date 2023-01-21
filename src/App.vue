<script setup lang="ts">
import PageComposition from './components/PageComposition.vue';
import AnimationFooter from './components/AnimationFooter.vue';
</script>

<template>
  <div class="main">
    <PageComposition />
  </div>
  <div class="footer">
    <AnimationFooter />
  </div>
</template>


<style lang="scss" scoped>
.main {
  position: relative;
}

.footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 2.5rem;  
  z-index: 70; 
}
</style>
