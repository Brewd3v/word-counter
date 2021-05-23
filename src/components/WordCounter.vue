<template>
<div class="word-counter-container">
  <div class="words-container">
    <h1>Word counter</h1>
    <div class="words">
      {{words ? words.trim().split(/\s+/).length : 0}}
    </div>
  </div>
  <div class="textarea-container">
    <textarea 
      v-model="words"
      placeholder="Type some awesome text here..."
    />
  </div>
</div>
</template>

<script>
export default {
  name: 'WordCounter',
  data(){
    return{
      words: ""
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1{
    font-weight: 700;
    font-size: 4rem;
    letter-spacing: -0.07em;
    margin: 20px 0;
}


.word-counter-container{
  width: 500px;
  padding: 20px;
}

.words-container{
  text-align: center;
}

.words{
  font-weight: 400;
  font-size: 100px;
  line-height: 1;
  letter-spacing: -0.05em;
  margin-bottom: 20px;
}

textarea{
  min-width: 100%;
  max-width: 100%;
  min-height: 300px;
  border-radius: 6px;
  padding: 15px;
  font-size: 18px;
  background-image: linear-gradient(to left, violet, indigo, green, blue, yellow, orange, red);
  -webkit-background-clip: text;
  -moz-background-clip: text;
  background-clip: text;
  color: transparent;
}

</style>
