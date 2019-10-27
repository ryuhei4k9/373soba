<template>
  <div class="wrapper">
    <section
      class="hero w-full bg-cover text-center flex flex-col items-center justify-center"
    >
      <h3 class="text-white mx-auto max-w-sm font-bold text-4xl">
        そばの記録
      </h3>
    </section>

    <section class="py-4">
      <div
        class="container max-w-4xl m-auto flex flex-wrap items-center justify-start"
      >
        <div class="w-full md:w-1/2 lg:w-1/3 flex flex-col mb-8 px-3">
          <div
            class="overflow-hidden bg-white rounded-lg shadow hover:shadow-raised hover:translateY-2px transition"
          >
            <img
              class="w-full"
              src="~/assets/images/tamanoya.jpg"
              alt="玉乃屋"
            />
            <div class="px-6 py-4 flex flex-col justify-between">
              <h3 class="font-bold text-gray-900 mb-4 leading-normal">
                玉乃屋
              </h3>
              <p class="inline-flex items-center text-xs">
                <span
                  class="bg-indigo-900 text-white mr-2 px-3 py-1 rounded-full"
                >
                  調布市
                </span>
                <span
                  class="bg-indigo-900 text-white mr-2 px-3 py-1 rounded-full"
                >
                  深大寺
                </span>
              </p>
            </div>
          </div>
        </div>
        <div class="w-full md:w-1/2 lg:w-1/3 flex flex-col mb-8 px-3">
          <div
            class="overflow-hidden bg-white rounded-lg shadow hover:shadow-raised hover:translateY-2px transition"
          >
            <img
              class="w-full"
              src="~/assets/images/hyakusoba.jpg"
              alt="浅草橋 百そば"
            />
            <div class="px-6 py-4 flex flex-col justify-between">
              <h3 class="font-bold text-gray-900 mb-4 leading-normal">
                浅草橋 百そば
              </h3>
              <p class="inline-flex items-center text-xs">
                <span
                  class="bg-indigo-900 text-white mr-2 px-3 py-1 rounded-full"
                >
                  台東区
                </span>
                <span
                  class="bg-indigo-900 text-white mr-2 px-3 py-1 rounded-full"
                >
                  浅草橋
                </span>
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  components: {}
}
</script>

<style scoped>
.wrapper {
  font-family: 'Noto Sans JP', serif;
  background-color: #f4f7f5;
}

.hero {
  background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
    url(~@/assets/images/tamanoya_shop.jpg);
  background-repeat: no-repeat;
  height: 50vh;
}
</style>
