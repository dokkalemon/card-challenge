<template>
  <div class="app">
    
    <Card />
  </div>
</template>

<script>
import Card from '@/components/Card.vue'

export default {
  name: 'App',

  components: {
    Card,
    
  }
}
</script>

<style lang="scss">
@import '@/styles/utilities';
@import '@/styles/vars';

.app {
  height: 100vh;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  

}

</style>
