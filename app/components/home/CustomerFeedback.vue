<template>
  <section class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-4">
      <!-- Tiêu đề -->
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold text-red-500">
          Cảm Nhận Khách Hàng khi dùng Dịch vụ
        </h2>
        <div class="mt-2 w-20 h-1 bg-red-500 mx-auto"></div>
      </div>

      <!-- Danh sách đánh giá -->
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <div
          v-for="(feedback, index) in feedbacks"
          :key="index"
          class="bg-white p-6 rounded-2xl shadow-sm border text-gray-700 space-y-4"
        >
          <!-- Nội dung -->
          <p>{{ feedback.text }}</p>

          <!-- Rating -->
          <div class="text-red-500 text-sm">
            <span v-for="i in 5" :key="i">
              <i class="fas fa-star"></i>
            </span>
          </div>

          <!-- Người dùng -->
          <div class="flex items-center gap-3 pt-2">
            <img
              :src="feedback.avatar"
              alt="avatar"
              class="w-10 h-10 rounded-full object-cover"
            />
            <div class="text-sm font-bold text-red-500 flex items-center gap-1">
              {{ feedback.name }}
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const feedbacks = [
  {
    text: "Tôi rất hài lòng với dịch vụ thiết kế kiến trúc của Nhà Thầu Vàng. Đội ngũ làm việc chuyên nghiệp, lắng nghe và biến ý tưởng của tôi thành bản vẽ hoàn hảo. Rất đáng tin cậy!",
    name: "Anh Minh (Q.7, TP.HCM)",
    avatar: "images/avt_1.png",
  },
  {
    text: "Từ khâu tư vấn đến khi bàn giao công trình, mọi thứ đều rõ ràng và đúng tiến độ. Thi công chắc chắn, nội thất đẹp, giá hợp lý. Gia đình tôi rất ưng ý!",
    name: "Chị Hương (Bình Thạnh)",
    avatar: "images/avt_2.png",
  },
  {
    text: "Dịch vụ trọn gói nên tôi không phải lo lắng gì nhiều. Thiết kế 3D chi tiết, chọn vật liệu được tư vấn kỹ. Nhà vừa đẹp vừa tiện nghi, đúng như mong đợi.",
    name: "Anh Tài (Thủ Đức)",
    avatar: "images/avt_3.png",
  },
];
</script>

<style scoped>
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css");
</style>
