<script setup>
import { ref } from "vue";

const name = ref("");

function addName() {
  name.value = "";
}
</script>

<template>
  <h2>Player's Name is: {{ name }}</h2>
  <form @submit.prevent="addName">
    <input v-model="name" required placeholder="name..." />
    <!-- <button>Add Name</button> -->
  </form>
</template>
