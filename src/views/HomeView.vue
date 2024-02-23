<template>
  <div class="home">
    <h1 class="logo">Broken Sweatshirt</h1>
    <button @click="playAudio">Click Here!</button>


  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'HomeView',
  methods: {
    playAudio() {
      const audio = new Audio(require('@/assets/yeah.mp3'));
      audio.play();
    }
  }
}
</script>
