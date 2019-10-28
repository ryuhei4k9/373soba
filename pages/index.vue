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
        <div
          v-for="shop of shops"
          :key="shop.id"
          class="w-full md:w-1/2 lg:w-1/3 flex flex-col mb-8 px-3"
        >
          <soba-card :shop="shop" />
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import SobaCard from '~/components/SobaCard'
import shops from '~/assets/json/shops.json'

export default {
  components: { SobaCard },
  data() {
    return {
      shops
    }
  }
}
</script>

<style scoped>
.wrapper {
  font-family: 'Noto Sans JP', serif;
  background-color: #fefded;
}

.hero {
  background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
    url(~@/assets/images/tamanoya_shop.jpg);
  background-repeat: no-repeat;
  height: 50vh;
}
</style>
