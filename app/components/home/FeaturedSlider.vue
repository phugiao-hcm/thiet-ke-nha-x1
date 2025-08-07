<template>
  <section class="bg-white py-20 px-6 relative">
    <div class="max-w-screen-xl mx-auto">
      <!-- Heading -->
      <div class="mb-12">
        <h2 class="text-4xl font-bold text-black mb-3">Dự án mới nhất</h2>
        <p class="text-gray-500 text-lg max-w-2xl">
          Các dự án của chúng tôi mang dấu ấn riêng trong kiến trúc đã góp phần
          biến căn nhà trong mơ của khách hàng thành hiện thực.
        </p>
      </div>

      <!-- Triangle image left -->
      <div
        class="absolute left-0 top-1/2 transform -translate-y-1/2 hidden md:block"
      >
        <svg viewBox="0 0 100 100" class="w-48 h-auto">
          <defs>
            <clipPath id="triangleClip2">
              <polygon points="50,0 100,100 0,100" />
            </clipPath>
          </defs>
          <image
            xlink:href="/images/avt_1.png"
            width="100"
            height="100"
            preserveAspectRatio="xMidYMid slice"
            clip-path="url(#triangleClip2)"
          />
          <polygon
            points="50,0 100,100 0,100"
            fill="none"
            stroke="orange"
            stroke-width="3"
          />
        </svg>
      </div>

      <!-- Dự án: Waterpoint Bến Lức -->
      <div class="mb-10">
        <div class="flex justify-between items-center mb-4">
          <h3 class="text-2xl font-semibold">Waterpoint Bến Lức</h3>
          <NuxtLink
            to="/du-an"
            class="bg-orange-500 hover:bg-orange-600 text-white px-4 py-2 rounded-full text-sm"
          >
            Xem toàn bộ
          </NuxtLink>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
          <img
            src="/images/nha_1.png"
            alt="project 1"
            class="rounded-lg shadow-md"
          />
          <img
            src="/images/nha_2.png"
            alt="project 2"
            class="rounded-lg shadow-md"
          />
          <img
            src="/images/nha_3.png"
            alt="project 3"
            class="rounded-lg shadow-md"
          />
        </div>
      </div>

      <!-- Dự án: Tp Thủ Đức -->
      <div class="mb-4">
        <h3 class="text-2xl font-semibold mb-4">Tp Thủ Đức</h3>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
          <img
            src="/images/nha_2.png"
            alt="project 4"
            class="rounded-lg shadow-md"
          />
          <img
            src="/images/nha_5.png"
            alt="project 5"
            class="rounded-lg shadow-md"
          />
          <img
            src="/images/nha_6.png"
            alt="project 6"
            class="rounded-lg shadow-md"
          />
        </div>
      </div>

      <div class="flex justify-end mt-6">
        <NuxtLink
          to="/"
          class="bg-orange-500 hover:bg-orange-600 text-white px-4 py-2 rounded-full text-sm"
        >
          Xem toàn bộ
        </NuxtLink>
      </div>
    </div>
  </section>
</template>

<script setup>
// No script logic needed here
</script>
