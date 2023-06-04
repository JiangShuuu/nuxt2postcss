<template>
  <div>
    <div class="w-full h-full">
      <div class="bg-[#fbc3a7] text-center">
        <p class="text-[32px] mb-6 md:text-[42px]">Hello, BEM!</p>
        <p class="text-2xl md:text-[32px]">Hello, SubBEM!</p>
      </div>
    </div>
    <div class="w-full h-full mt-4">
      <div class="flex items-center space-x-2 justify-center">
        <div class="text-2xl mb-2.5 text-center md:text-[32px]">我是內容</div>
        <nuxt-link to="/scss">到 scss 頁面</nuxt-link>
      </div>
      <div class="flex flex-wrap">
        <div class="w-1/5 bg-[#f2f2f2] p-2.5 mr-2.5 mb-5">
          <div class="mb-2">選項 1</div>
          <div class="mb-2">選項 2</div>
          <div class="mb-2">選項 3</div>
          <div class="mb-2">選項 4</div>
        </div>
        <div
          class="w-4/5 flex-1 grid grid-cols-2 gap-4 justify-items-center md:grid-cols-3"
        >
          <div
            class="relative w-[150px] mb-5 p-6 bg-[#f2f2f2] cursor-pointer flex flex-col items-center justify-center"
          >
            <div
              class="w-[100px] h-[100px] text-center bg-[#0000FF] text-white"
            >
              卡片內容
            </div>
            <h3
              class="text-[18px] mb-2 ani hover:text-[#FF0000] lg:hover:text-[#008000]"
            >
              主標題 1
            </h3>
            <p class="text-sm ani hover:text-[#0000FF]">副標題 1</p>
            <img
              src="~/assets/img/heart.png"
              class="w-4 h-4 absolute top-1.5 right-1"
            />
          </div>
          <div
            class="relative w-[150px] mb-5 p-6 bg-[#f2f2f2] cursor-pointer flex flex-col items-center justify-center"
          >
            <div
              class="w-[100px] h-[100px] text-center bg-[#0000FF] text-white"
            >
              卡片內容
            </div>
            <h3
              class="text-[18px] mb-2 ani hover:text-[#FF0000] lg:hover:text-[#008000]"
            >
              主標題 2
            </h3>
            <p class="text-sm ani hover:text-[#0000FF]">副標題 2</p>
            <img
              src="~/assets/img/heart.png"
              class="w-4 h-4 absolute top-1.5 right-1"
            />
          </div>
          <div
            class="relative w-[150px] mb-5 p-6 bg-[#f2f2f2] cursor-pointer flex flex-col items-center justify-center"
          >
            <div
              class="w-[100px] h-[100px] text-center bg-[#0000FF] text-white"
            >
              卡片內容
            </div>
            <h3
              class="text-[18px] mb-2 ani hover:text-[#FF0000] lg:hover:text-[#008000]"
            >
              主標題 3
            </h3>
            <p class="text-sm ani hover:text-[#0000FF]">副標題 3</p>
            <img
              src="~/assets/img/heart.png"
              class="w-4 h-4 absolute top-1.5 right-1"
            />
          </div>
          <div
            class="relative w-[150px] mb-5 p-6 bg-[#f2f2f2] cursor-pointer flex flex-col items-center justify-center"
          >
            <div
              class="w-[100px] h-[100px] text-center bg-[#0000FF] text-white"
            >
              卡片內容
            </div>
            <h3
              class="text-[18px] mb-2 ani hover:text-[#FF0000] lg:hover:text-[#008000]"
            >
              主標題 4
            </h3>
            <p class="text-sm ani hover:text-[#0000FF]">副標題 4</p>
            <img
              src="~/assets/img/heart.png"
              class="w-4 h-4 absolute top-1.5 right-1"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
