<template>
  <div class="app-a">
    {{ count }}
    <button @click="handleAdd">+1</button>
  </div>
</template>

<script setup>
  import { ref } from 'vue';
  const count = ref(0);

  const handleAdd = () => {
    count.value += 1;
  };
</script>

<style lang="less" scoped>
  .app-a {
    margin-top: 20px;
  }
</style>
