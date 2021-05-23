<template>
  <WordCounter />
</template>

<script>
import WordCounter from './components/WordCounter.vue'

export default {
  name: 'App',
  components: {
    WordCounter
  }
}
</script>

<style>
*{
  box-sizing: border-box;
}  
body{
  margin: 0;
  font-family: 'Inter';
}


#app {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background: #ffffff;
}
</style>
