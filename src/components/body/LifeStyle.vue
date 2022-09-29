<template>
  <div class="lifestyle">
    <div class="banner-title">
      <a href="#" class="label bold hover-blue">Lifestyle</a>
      <a href="" class="view-all">View all</a>
    </div>
    <div class="post-content flex">
      <div
        v-for="(data, index) in lifeSylesData"
        :key="index"
        class="post-card"
      >
        <img class="cursor-pointer" :src="data.image" alt="post card" />
        <div class="routes bold text-uppercase">
          <a href="">Thời gian</a>, <a href="">Lifestyle</a>
        </div>
        <div class="large-width">
          <a href="" class="title bold hover-blue">{{ data.title }}</a>
          <p class="time hover-underline">{{ data.date }}</p>
        </div>
        <span class="introduce">{{ data.description }}</span>
        <a href="" class="read-more">Read more</a>
        <div class="small-posts">
          <div
            v-for="(post, index_02) in data.smallPosts"
            :key="index_02"
            class="small-post flex"
          >
            <img class="cursor-pointer" :src="post.image" alt="small post" />
            <div class="">
              <a href="" class="title bold hover-blue">{{ post.title }}</a>
              <p class="time hover-underline">{{ post.date }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      lifeSylesData: [
        {
          image:
            "https://xinhxinh.vn/wp-content/uploads/2021/10/trang-phuc-dao-pho_28-800x500.jpg",
          title: "Học lỏm 5 cách phối đồ dành cho trang phục dạo phố",
          date: "16/12/2021",
          description:
            "Trang phục dạo phố là những trang phục được mọi người diện thường xuyên, đủ loại phong cách và thể hiện được thời trang riêng biệt của mỗi người. Outfit dạo phố ưu tiên sự thoải mái, năng động, có một chút xíu tùy ý, thảnh thơi",
          smallPosts: [
            {
              image:
                "https://xinhxinh.vn/wp-content/uploads/2021/09/trang-phuc-du-lich-sang-trong-150x150.jpg",
              title: "Bật mí 18+ kiểu trang phục du lịch sang trọng",
              date: "19/09/2021",
            },
            {
              image:
                "https://xinhxinh.vn/wp-content/uploads/2021/09/Goi-y-19-cach-mix-do-voi-ao-len-hot-nhat-2021-150x150.jpg",
              title: "Gợi ý 19+ cách mix đồ với áo len hot nhất 2021",
              date: "14/09/2021",
            },
          ],
        },
        {
          image:
            "https://xinhxinh.vn/wp-content/uploads/2021/09/Cach-mix-do-de-thuong-cho-co-nang-cong-so-800x500.jpg",
          title: "19+ cách mix đồ dễ thương cho cô nàng công sở",
          date: "24/09/2021",
          description:
            "Bạn là một cô nàng công sở nhưng đã chán ngán với những phong cách thường ngày của mình và đang muốn “đổi gió” phong cách thời trang của mình. Đôi khi chúng ta chỉ chỉ cần mix một số items đơn giản với nhau thì đã có thể nâng tầm trang phục của mình và tạo ra những set đồ đẹp để nàng diện đi làm rồi đấy!",
          smallPosts: [
            {
              image:
                "https://xinhxinh.vn/wp-content/uploads/2021/09/Bo-tui-19-Cach-phoi-blazer-phong-cach-cho-nang-xuong-pho-150x150.jpg",
              title:
                "Bỏ túi 19+ Cách phối blazer phong cách cho nàng xuống phố",
              date: "18/09/2021",
            },
            {
              image:
                "https://xinhxinh.vn/wp-content/uploads/2021/09/Bat-mi-17-cach-dong-sovin-dep-150x150.jpg",
              title: "Bật mí 17+ cách đóng sơ vin đẹp cực chất",
              date: "12/09/2021",
            },
          ],
        },
      ],
    };
  },
};
</script>

<style></style>
