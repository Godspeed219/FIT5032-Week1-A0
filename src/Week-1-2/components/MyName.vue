<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="greetings">
    <h1>{{ msg }}</h1>
    <h3>Hey there! I'm <span class="highlight">Palash Rambhia</span>.</h3>
  </div>
</template>

<style scoped>
.greetings {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

h1 {
  font-weight: 600;
  font-size: 5rem;
  color: #10b981;
  margin-bottom: 0.5rem;
  margin-top: 1rem;
}

h3 {
  font-size: 1.25rem;
  font-weight: 400;
  color: #10b981;
}

.highlight {
  font-weight: 600;
  color: #ffffff;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
