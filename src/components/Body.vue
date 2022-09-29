<template>
  <div class="body">
    <TopImages :TopLabelData="data[0]" />
    <ChamSocDa />
    <LifeStyle />
    <KieuTocDep />
    <TopImages :TopLabelData="data[1]" />
    <Nail />
  </div>
</template>

<script>
import TopImages from "./body/TopImages.vue";
import ChamSocDa from "./body/ChamSocDa.vue";
import LifeStyle from "./body/LifeStyle.vue";
import KieuTocDep from "./body/KieuTocDep.vue";
import Nail from "./body/Nail.vue";
export default {
  components: {
    TopImages,
    ChamSocDa,
    LifeStyle,
    KieuTocDep,
    Nail,
  },
  data() {
    return {
      data: [
        [
          {
            date: "31/12/2021",
            description:
              "Ngọt ngào với 18+ trang phục màu hồng đáng yêu cực kì nữ tính",
          },
          {
            date: "31/12/2021",
            description:
              "Lấy lại tự tin với 18+ kiểu trang phục cho cô nàng vai rộng siêu nữ tính",
          },
          {
            date: "31/12/2021",
            description:
              "Ngọt ngào với 18+ trang phục màu hồng đáng yêu cực kì nữ tính",
          },
          {
            date: "25/12/2021",
            description:
              "15 cách chăm sóc tóc mềm mượt, chắc khoẻ cực đơn giản",
          },
        ],
        [
          {
            date: "1/12/2021",
            description:
              "Ngọt ngào với 18+ trang phục màu hồng đáng yêu cực kì nữ tính abcdd",
          },
          {
            date: "31/12/2021",
            description:
              "Lấy lại tự tin với 18+ kiểu trang phục cho cô nàng vai rộng siêu nữ tính",
          },
          {
            date: "31/12/2021",
            description:
              "Ngọt ngào với 18+ trang phục màu hồng đáng yêu cực kì nữ tính",
          },
          {
            date: "25/12/2021",
            description:
              "15 cách chăm sóc tóc mềm mượt, chắc khoẻ cực đơn giản",
          },
        ],
      ],
    };
  },
};
</script>

<style></style>
