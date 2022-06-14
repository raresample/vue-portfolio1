<template>
  <div class="container">
    <img id="headshot" src="https://picsum.photos/468" alt="Aaron Hope photo">
    <HelloWorld id="helloworld" msg="Aaron Hope, at your service"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>

<style scoped>
#headshot {
  margin-bottom: 2rem;
  max-width: 90%;
}

@media(min-width:769px) {
  #headshot {
    float: left;
    width: 50%;
    box-sizing: border-box;
  }
  #helloworld {
    float: right;
    width: 50%;
    padding: 0 30px;
    box-sizing: border-box;
  }
}


</style>