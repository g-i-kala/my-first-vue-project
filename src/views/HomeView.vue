<script setup>
import { ref } from 'vue'
import TheWelcome from '../components/TheWelcome.vue'

const message = ref("Hello bijacz!");

let doSomething = () => {
  alert("doing it yess!");
}
</script>

<template>
  <main>
    <TheWelcome />
    <p>
      <button @click="doSomething">Click Me!</button>
    </p>
    <p>{{ message }}</p>
    <input type="text" v-model="message" />

  </main>
</template>
