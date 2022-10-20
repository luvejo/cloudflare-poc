<script setup>
const res = await useFetch(
  "https://strangerthings-quotes.vercel.app/api/quotes/5",
  {
    method: "get",
  }
);
</script>

<template>
  <div>
    {{ res?.data }}
  </div>
</template>
