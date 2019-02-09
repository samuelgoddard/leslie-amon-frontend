<template>
  <a href="#" class="m-product-teaser block no-underline text-black hover:underline group">
    <div class="overflow-hidden bg-grey-lightest mb-2">
      <img :src="image" alt="Product Image" class="w-full mb-0 block group-hover:scale-1 transition relative" />
    </div>
    <span class="block text-black text-lg">{{ title }}</span>
    <span class="block text-grey-dark text-sm">{{ price }}&euro;</span>
  </a>
</template>

<script>
export default {
  props: {
    title: String,
    price: String,
    image: String
  }
}
</script>