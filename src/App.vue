<template>
  <div class="app">
    
    <Card 
    title="Equilibrium #3429"
    text="Our Equilibrium collection promotes balance and calm."
    value="0.041ETH"
    date="3 days left"
    name="Jules Wyvern"
    thumb="image-equilibrium.jpg"
    avatar="image-avatar.png"
    />
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
