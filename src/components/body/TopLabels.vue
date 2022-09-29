<template>
  <div class="top-labels">
    <p class="bold white-text text-center">{{ data.date }}</p>
    <h2 class="bold white-text text-center">
      {{ data.description }}
    </h2>
  </div>
</template>

<script>
export default {
    props:{
        data: Object
    }
};
</script>

<style></style>
