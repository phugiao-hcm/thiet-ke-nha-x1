<template>
  <section class="news-section max-w-screen-xl mx-auto py-16">
    <div class="flex items-center justify-between mb-12">
      <h2 class="text-3xl font-semibold uppercase">
        Tin tức - sự kiện của <span class="text-red-500">Hiashi</span>
      </h2>
      <NuxtLink
        to="/tin-tuc"
        class="flex items-center text-gray-700 hover:text-red-500 transition"
      >
        <span class="mr-2">Xem tất cả</span>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M9 5l7 7-7 7"
          />
        </svg>
      </NuxtLink>
    </div>

    <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
      <div v-for="post in posts" :key="post.id" class="space-y-4 group">
        <NuxtLink :to="post.link" class="block overflow-hidden rounded">
          <img
            :src="post.image"
            :alt="post.title"
            class="w-full h-56 object-cover transition-transform group-hover:scale-105"
          />
        </NuxtLink>
        <p class="text-gray-500 text-sm">{{ post.date }}</p>
        <NuxtLink :to="post.link">
          <h3 class="font-bold text-lg hover:text-red-500 transition">
            {{ post.title }}
          </h3>
        </NuxtLink>
        <p class="text-gray-600 text-sm">{{ post.description }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
const posts = [
  {
    id: 1,
    image: "/images/news_1.png",
    date: "21/09/2023",
    title: "Giải pháp xanh cho hệ kết cấu cùng Glubam (Glued Laminated Bamboo)",
    description:
      "Từ xa xưa con người đã biết sử dụng gỗ như là vật liệu chính trong xây dựng...",
    link: "/tin-tuc/giai-phap-xanh-glubam",
  },
  {
    id: 2,
    image: "/images/news_2.png",
    date: "31/08/2023",
    title: "Có nên sử dụng sàn nhựa Vinyl?",
    description:
      "Trong quá trình tìm kiếm vật liệu, chắc hẳn bạn đã nghe đến sàn nhựa Vinyl...",
    link: "/tin-tuc/co-nen-su-dung-san-nhua-vinyl",
  },
  {
    id: 3,
    image: "/images/news_3.png",
    date: "20/09/2023",
    title: "Gỗ tre thông minh - ứng dụng đa chiều",
    description: "HiYo vừa cập nhật thêm những sản phẩm độc đáo...",
    link: "/tin-tuc/go-tre-thong-minh",
  },
  {
    id: 4,
    image: "/images/news_4.png",
    date: "31/08/2023",
    title: "Cẩm nang mua sàn gỗ an toàn",
    description:
      "Sàn gỗ nhân tạo có hại sức khỏe hay không? Làm sao chọn sàn an toàn?",
    link: "/tin-tuc/cam-nang-san-go-an-toan",
  },
];
</script>

<style scoped>
.news-section h2 {
  border-top: 3px solid #e53e3e; /* màu đỏ gần giống chữ "Hiashi" */
  display: inline-block;
  padding-top: 0.5rem;
}
</style>
