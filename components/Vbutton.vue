<template>
  <a :href="url" class="bg-red-600 hover:bg-red-700 text-white">
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
  font-size: 16px;
  padding: 0.5rem 1rem;
  border-radius: 1.5rem;
}
</style>
