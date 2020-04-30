<template>
  <a :href="url" class="bg-red-400 hover:bg-red-500 text-white">
    <font-awesome-icon :icon="['fa', icon]" class="text-white" />
    {{ content }}
  </a>
</template>

<script>
export default {
  name: 'Vbutton',
  props: {
    content: String,
    url: String,
    icon: String
  }
}
</script>
<style scoped>
a {
  padding: 0.5rem 1rem;
  border-radius: 0.5rem;
}
</style>
