<template>

  <div class="block">
    <div>
      <img src= 'uImage' alt="">
    </div>

    <div>
      <a :href="url" class="bg-red-600 hover:bg-red-500 text-white">
          <font-awesome-icon :icon="['fa', icon]" class="text-white" />
          {{ vContent }}
      </a>
    </div>
    
    <div>
      <p>{{content}}</p>
    </div>
    
  </div>
</template>
<script>
export default {
  name: 'YoQuiero',
  props: {
    vContent: String,
    content: String,
    uImage: String,
    url: String,
    icon: String
  }
}
</script>
<style scoped>

.block{
  display: grid;
  justify-content: center;
  align-items: center;
  border: 2px solid red;
  padding: 20px;

}

p{
  border: 2px solid blue;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  width: 200px;
  text-align: center;
}

.block div{
  display: grid;
  justify-content: center;
  align-items: center;
  border: 2px solid red;
  margin: 5px;
}


a {
  padding: 0.5rem ;
  border-radius: 1rem;
  border: 2px solid red;
  width: 100%;
  
}

img{
  width: 200px;
  height: 200px;
  display: block;
  border: 2px solid red;
  border-radius: 1rem;
}
</style>
