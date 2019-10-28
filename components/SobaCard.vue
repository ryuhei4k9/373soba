<template>
  <div
    class="overflow-hidden bg-white rounded-lg shadow hover:shadow-raised hover:translateY-2px transition"
  >
    <img class="w-full" src="~assets/images/tamanoya.jpg" alt="玉乃屋" />
    <div class="px-6 py-4 flex flex-col justify-between">
      <h3 class="font-bold text-gray-900 mb-4 leading-normal">
        {{ shop.shopName }}
      </h3>
      <p class="inline-flex items-center text-xs">
        <span class="bg-indigo-900 text-white mr-2 px-3 py-1 rounded-full">
          {{ shop.tags[0] }}
        </span>
        <span class="bg-indigo-900 text-white mr-2 px-3 py-1 rounded-full">
          {{ shop.tags[1] }}
        </span>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: ['shop'],
  computed: {
    imgSrc() {
      return require(this.shop.thumbnailUrl)
    }
  }
}
</script>

<style scoped></style>
