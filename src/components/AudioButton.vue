<template>
  <button @click="play">Click Me!</button>
</template>

<script>
import { useSound } from '@vueuse/sound'
import buttonSfx from '../assets/yeah.mp3'

export default {
  setup() {
    const { play } = useSound(buttonSfx)

    return {
      play,
    }
  },
}
</script>