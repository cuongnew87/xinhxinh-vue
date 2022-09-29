<template>
  <div class="top-images flex">
    <div class="left-image center-background cursor-pointer">
      <TopLabel :data="TopLabelData[0]" />
    </div>
    <div class="right-images">
      <div class="upper-image center-background cursor-pointer">
        <TopLabel :data="TopLabelData[1]" />
      </div>
      <div class="down-images flex">
        <div
          v-for="(data, index) in TopLabelData.slice(2, 4)"
          :key="index"
          class="down-image center-background cursor-pointer"
          :style="{ 'background-image': `url(${backgroundImages[index]})` }"
        >
          <TopLabel :data="data" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TopLabel from "./TopLabels.vue";
export default {
  components: {
    TopLabel,
  },
  data() {
    return {
      backgroundImages: [
        "https://xinhxinh.vn/wp-content/uploads/2021/12/trang-phuc-mau-hong-dang-yeu.png",
        "https://xinhxinh.vn/wp-content/uploads/2021/12/image-3.jpeg",
      ],
    };
  },
  props:{
    TopLabelData: Object
  }
};
</script>

<style></style>
