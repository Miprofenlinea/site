<template>
  <div>
    <nav class="img"></nav>
    <p>{{ content }}</p>
    <a :href="url" class="bg-red-400 hover:bg-red-500 text-white">
        <font-awesome-icon :icon="['fa', icon]" class="text-white" />
        {{ vContent }}
    </a>
  </div>
</template>
<script>
export default {
  name: 'YoQuiero',
  props: {
    vContent: String,
    content: String,
    urlImage: String,
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
.img {
  background-image: url('aprender.png');
}
</style>
