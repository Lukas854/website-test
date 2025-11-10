<script setup>
import {ref} from "vue";

const props = defineProps({
    text: {
      type: String,
      required: true,
    },
    tuerchenNummer: {
      type: Number,
      required: true,
    },
    bild: {
      type: String,
      required: false,
    }

  }
)
const isFlipped = ref(false)


function flip() {
  const today = new Date();
  const cardDate = new Date(2025, 12, props.tuerchenNummer);
  const todayString = today.toLocaleDateString('de-DE');

  if (today < cardDate) {
    alert(`Ätsch Bätsch - das Türchen darf noch nicht geöffnet werden. Heute ist doch erst der ${todayString}.`)
    return
  }
  isFlipped.value = !isFlipped.value
}
</script>

<template>
  <div class="flip-card" @click="flip">
    <div class="flip-card-inner" :class="{ flipped: isFlipped }">
      <!-- Vorderseite -->
      <div class="flip-card-front">
        <span v-if="text">Türchen Nummer: {{ tuerchenNummer }} | Öffne mich!</span>
      </div>

      <!-- Rückseite -->
      <div class="flip-card-back">
        <img src="../assets/logo.svg" alt="Logo"/>
        <span v-if="text">{{ text }}</span>
      </div>
    </div>
  </div>
</template>

<style scoped>
.flip-card {
  perspective: 1000px;
  width: 200px;
  height: 200px;
}

.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  transition: transform 0.6s;
  transform-style: preserve-3d;
}

.flip-card-inner.flipped {
  transform: rotateY(180deg);
}

.flip-card-front,
.flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: 2px solid darkgreen;
  padding: 7px;
  box-sizing: border-box;
}

.flip-card-back {
  transform: rotateY(180deg);
}
</style>
