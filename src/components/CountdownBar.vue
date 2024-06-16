<template>
  <div class="countdown-bar">
    <p class="values">
      {{ countdown.days }} : 
      {{ padWithZero(countdown.hours) }} : 
      {{ padWithZero(countdown.minutes) }} : 
      {{ padWithZero(countdown.seconds) }}
    </p>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const countdown = ref({
  days: 0,
  hours: 0,
  minutes: 0,
  seconds: 0
});

const updateCountdown = () => {
  const now = new Date().getTime();
  const startDate = "November 12, 2025 08:00:00";
  const timestamp = Date.parse(startDate);
  const distance = timestamp - now;

  countdown.value.days = Math.floor(distance / (1000 * 60 * 60 * 24));
  countdown.value.hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  countdown.value.minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  countdown.value.seconds = Math.floor((distance % (1000 * 60)) / 1000);
};

const padWithZero = (number) => {
  return number.toString().padStart(2, '0');
};

onMounted(() => {
  updateCountdown();
  setInterval(updateCountdown, 1000);
});
</script>

<style lang="scss" scoped>
@import '/src/assets/styles/styles.scss';

.countdown-bar {
    background-color: $countdown-background;
    height: 80px;
    top: 0;
    left: 0;
    position: fixed;
    width: 100%;
    margin: 0;
    padding: 0;
    text-align: center;
}

.values {
    font-size: 40px;
    font-family: Roboto, sans-serif;
    margin-top: -4px;
}

</style>