<template>
  <div class="h-screen">
    <div class="grid grid-cols-12 gap-3 h-full">
      <div class="hidden md:block col-span-3 h-full bg-art bg-cover bg-center bg-no-repeat" />
      <div class="col-span-12 md:col-span-9">
        <slot />
      </div>
    </div>
  </div>
</template>

<script setup>
useHead({
  htmlAttrs: {
    class: 'h-full'
  }
})
</script>

<style scoped>
.bg-art {
  background-image: url('https://images.unsplash.com/photo-1488485339565-566d63f7dbb7?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2787&q=80');
}
</style>