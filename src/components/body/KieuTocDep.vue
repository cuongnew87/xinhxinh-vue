<template>
  <div class="kieutocdep">
    <div class="banner-title">
      <a href="#" class="label bold hover-blue">Kiểu tóc đẹp</a>
      <a href="" class="view-all">View all</a>
    </div>
    <div class="content flex">
        <LeftBigPost :data="leftPostData" />
      <div class="right-content-cards">
        <div v-for="(post, index) in posts" :key="index" class="card flex">
          <img
            class="cursor-pointer"
            :src="post.image"
            alt="card"
          />
          <div>
            <a href="" class="bold hover-blue"
              >{{ post.title }}</a
            >
            <p class="time hover-underline">
              <i class="far fa-clock"></i>{{ post.date }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LeftBigPost from "./LeftBigPost.vue"
export default {
    components: {
    LeftBigPost
  },
  data() {
    return {
      posts: [
        {
          image:
            "https://xinhxinh.vn/wp-content/uploads/2021/07/kieu-toc-mai-dai-uon-nhe-520x400.jpg",
          title: "20+ kiểu tóc mái dài uốn nhẹ cân mọi gương mặt",
          date: "21/07/2021",
        },
        {
          image:
            "https://xinhxinh.vn/wp-content/uploads/2021/07/toc-mau-xanh-reu-thumb-520x400.jpg",
          title: "Tổng hợp 18+ tóc màu xanh rêu ấn tượng",
          date: "20/07/2021",
        },
        {
          image:
            "https://xinhxinh.vn/wp-content/uploads/2021/07/toc-mau-than-chi_12-520x400.jpg",
          title: "Lưu ngay 4 màu tóc than chì siêu HOT hiện nay",
          date: "19/07/2021",
        },
        {
          image:
            "https://xinhxinh.vn/wp-content/uploads/2021/07/kieu-toc-di-dam-cuoi-cuc-xinh-520x400.jpg",
          title: "Bỏ túi 20+ kiểu tóc đi đám cưới cực xinh “lấn át” cả cô dâu",
          date: "18/07/2021",
        },
      ],
      leftPostData:{
        title: 'Lưu ngay 19+ kiểu tóc cưới cho cô dâu sang xịn mịn cực xinh',
        image: 'https://xinhxinh.vn/wp-content/uploads/2021/07/Thiet-ke-khong-ten-2-800x500.png',
        description: 'Ngày cưới là ngày trọng đại nhất trong cuộc đời của mỗi cô dâu vì thế các nàng lại xúng xính chọn váy, lựa mẫu makeup thật xinh nhưng thường bỏ qua bước chọn kiểu tóc cưới.',
        date: '23/07/2021'
      }
    };
  },
};
</script>

<style></style>
