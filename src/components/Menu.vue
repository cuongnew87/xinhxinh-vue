<template>
  <div class="menu">
    <ul class="flex">
      <li v-for="(link, index) in links" :key="index"><a href="" class="bold text-uppercase hover-blue">{{ link }}</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      links: [
        "Chăm sóc da",
        "Trang điểm",
        "Thời trang",
        "Lifestyle",
        "Kiểu tóc",
        "Nail",
        "Mẹo hay",
      ],
    };
  },
};
</script>

<style></style>
