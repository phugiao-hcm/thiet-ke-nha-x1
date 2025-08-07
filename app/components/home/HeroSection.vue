<template>
  <section class="bg-white py-16 px-6">
    <div
      class="max-w-screen-xl mx-auto flex flex-col lg:flex-row items-center gap-10"
    >
      <!-- Left content -->
      <div class="lg:w-1/2">
        <h2 class="text-4xl font-extrabold text-black mb-4">
          Quy trình làm việc
        </h2>
        <p class="text-gray-600 mb-8">
          Nhà Thầu Vàng với mong muốn đem lại dịch vụ chất lượng tốt nhất, chúng
          tôi xây dựng quy trình Design & Build với hệ thống quản lý bằng công
          nghệ và nhân sự giàu kinh nghiệm giúp tiết kiệm thời gian và chi phí
          cho Chủ Đầu Tư
        </p>

        <!-- Steps -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <!-- Step 1 -->
          <div
            class="bg-gradient-to-br from-orange-400 to-orange-600 text-white p-6 rounded-xl shadow-md relative"
          >
            <h3 class="text-xl font-bold mb-2">Tư Vấn Dự Toán</h3>
            <p class="text-sm">
              Khi nhận được Yêu cầu của Chủ Đầu Tư, Nhà Thầu Vàng sẽ Tư vấn về
              thiết kế kiến trúc, kinh phí xây dựng.. hoàn toàn
              <strong>Miễn phí</strong>.
            </p>
            <span
              class="absolute top-4 right-4 text-4xl font-extrabold opacity-20"
              >1</span
            >
          </div>

          <!-- Step 2 -->
          <div class="bg-white p-6 rounded-xl shadow-md relative">
            <h3 class="text-xl font-semibold text-gray-800 mb-2">
              Thiết Kế Kiến Trúc
            </h3>
            <p class="text-sm text-gray-600">
              Chủ Đầu Tư và KTS cùng làm việc chi tiết về Mặt bằng, Thiết kế 3D,
              Hồ sơ triển khai thi công thật kỹ lưỡng kèm giải pháp thi công
              <strong>Thiết Thực</strong>.
            </p>
            <span
              class="absolute top-4 right-4 text-4xl font-extrabold text-orange-100"
              >2</span
            >
          </div>

          <!-- Step 3 -->
          <div class="bg-white p-6 rounded-xl shadow-md relative">
            <h3 class="text-xl font-semibold text-gray-800 mb-2">
              Thi Công Xây Dựng
            </h3>
            <p class="text-sm text-gray-600">
              Nhà Thầu Vàng hỗ trợ xin phép xây dựng, đăng ký thi công.
              <strong
                >Quay phim, chụp ảnh, báo cáo tiến độ thi công mỗi ngày</strong
              >. Đảm bảo kiểm soát tiến độ và chất lượng thi công tại Công
              trình.
            </p>
            <span
              class="absolute top-4 right-4 text-4xl font-extrabold text-orange-100"
              >3</span
            >
          </div>

          <!-- Step 4 -->
          <div class="bg-white p-6 rounded-xl shadow-md relative">
            <h3 class="text-xl font-semibold text-gray-800 mb-2">
              Nghiệm Thu Hoàn công
            </h3>
            <p class="text-sm text-gray-600">
              Kỹ sư gửi <strong>Bản nghiệm thu</strong> chuyên bước từng hạng
              mục. Chủ đầu tư có bất kỳ yêu cầu chỉnh sửa hay thay đổi, Nhà Thầu
              Vàng sẽ ghi nhận.
            </p>
            <span
              class="absolute top-4 right-4 text-4xl font-extrabold text-orange-100"
              >4</span
            >
          </div>
        </div>
      </div>

      <!-- Right content: Triangle image -->
      <div class="lg:w-1/2 flex justify-center relative w-full">
        <svg viewBox="0 0 100 100" class="w-[300px] md:w-[400px] h-auto">
          <defs>
            <clipPath id="triangleClip">
              <polygon points="50,0 100,100 0,100" />
            </clipPath>
          </defs>

          <image
            xlink:href="/images/avt_1.png"
            width="100"
            height="100"
            preserveAspectRatio="xMidYMid slice"
            clip-path="url(#triangleClip)"
          />

          <!-- Orange triangle stroke -->
          <polygon
            points="50,0 100,100 0,100"
            fill="none"
            stroke="orange"
            stroke-width="5"
          />
        </svg>
      </div>
    </div>
  </section>
</template>

<script setup>
// No JS needed for this component
</script>

<style scoped>
</style>
