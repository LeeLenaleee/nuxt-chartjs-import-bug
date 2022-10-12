<template>
  <h1>Test123</h1>
  <canvas id="ff"></canvas>
  <h2>Test321</h2>
</template>

<script setup lang="ts">
import { Chart, registerables } from "chart.js";


  Chart.register(...registerables);
  new Chart("ff", {
    type: "doughnut",
    data: {
      labels: ["chart", "js"],
      datasets: [
        {
          data: [2, 5],
        },
      ],
    },
  });
</script>
