<template>
  <div class="h-screen flex items-center justify-center">
    <spinner />
  </div>
</template>

<script setup>
useHead({
  title: 'Loading Nuxt3 Contacts',
  htmlAttrs: {}
})

onMounted(() => {
  setTimeout(() => {
    useRouter().replace({ path: '/signin' })
  }, 1000)
})
</script>
