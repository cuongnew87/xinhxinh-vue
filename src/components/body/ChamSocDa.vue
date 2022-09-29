<template>
  <div class="chamsocda">
    <div class="banner-title">
      <a href="#" class="label text-uppercase bold hover-blue">Chăm sóc da</a>
      <a href="" class="view-all">View all</a>
    </div>
    <div class="content flex">
      <LeftBigPost :data="leftPostData" />
      <div class="right-content">
        <div v-for="(data, index) in chamsocdaData" :key="index" class="card">
          <img
            class="cursor-pointer"
            :src="data.image"
            alt="card"
          />
          <a href="" class="bold hover-blue"
            >{{ data.title }}</a
          >
          <p class="time hover-underline">
            <i class="far fa-clock"></i>{{ data.date }}
          </p>
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
      chamsocdaData: [
        {
          image:
            "https://xinhxinh.vn/wp-content/uploads/2021/11/8-cach-lam-trang-da-trong-1-dem-hieu-qua-hiem-nguoi-biet-520x400.png",
          title: "8 cách làm trắng da trong 1 đêm hiệu quả hiếm người biết",
          date: "16/12/2021",
        },
        {
          image:
            "https://xinhxinh.vn/wp-content/uploads/2021/06/9-sai-lam-khi-rua-mat-khien-da-khong-lao-hoa-nhanh-chong-520x400.jpg",
          title: "9 sai lầm khi rửa mặt khiến da không lão hóa nhanh chóng",
          date: "01/07/2021",
        },
        {
          image:
            "https://xinhxinh.vn/wp-content/uploads/2021/06/Review-5-loai-mat-na-giay-Han-Quoc-duoc-chi-em-tin-dung-520x400.jpg",
          title: "Review 5 loại mặt nạ giấy Hàn Quốc được chị em tin dùng",
          date: "22/06/2021",
        },
        {
          image:
            "https://xinhxinh.vn/wp-content/uploads/2021/05/chon-kem-chong-nang-phu-hop-520x400.jpg",
          title: "Cách chọn kem chống nắng phù hợp với từng loại da",
          date: "05/06/2021",
        },
      ],
      leftPostData:{
        title: 'Hiểu rõ nguyên nhân khiến bạn skincare chưa hiệu quả',
        image: 'https://xinhxinh.vn/wp-content/uploads/2021/12/nguyen-nhan-khien-ban-skincare-chua-hieu-qua.jpg',
        description: 'Có rất nhiều nguyên nhân khiến quá trình skincare của bạn chưa được như ý muốn và rất có thể là do bạn hiểu sai kiến thức hay sử dụng sai trình tự sản phẩm. Cùng mình tìm hiểu nguyên nhân để bạn có thể skincare đúng nhé!',
        date: '16/12/2021'
      }
    };
  },
};
</script>

<style></style>
