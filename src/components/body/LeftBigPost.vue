<template>
  <div class="left-content">
    <img
      class="cursor-pointer"
      :src="data.image"
      alt=""
    />
    <a href="" class="link bold hover-blue"
      >{{data.title}}</a
    >
    <p class="time hover-underline"><i class="far fa-clock"></i>{{data.date}}</p>
    <span class="introduce"
      >{{data.description}}</span
    >
    <a href="" class="read-more">Read more</a>
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
