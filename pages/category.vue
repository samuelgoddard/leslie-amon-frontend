<template>
  <div>
    <!-- Page Title -->
    <section class="m-page-title w-full py-8 md:py-16 mb-10 md:mb-12">
      <div class="container">
        <div class="w-full">
          <h1 class="text-black font-light text-3xl md:text-4xl lg:text-5xl">Swimwear</h1>
        </div>
      </div>
      <div class="container">
        <div class="w-full">
          <div class="m-category-switcher flex flex-wrap">
            <a href="#" class="text-black mr-3 md:mr-5">All</a>
            <a href="#" class="text-grey-dark no-underline hover:text-black hover:underline mr-3 md:mr-5">One Piece</a>
            <a href="#" class="text-grey-dark no-underline hover:text-black hover:underline mr-3 md:mr-5">Bikini</a>
            <a href="#" class="text-grey-dark no-underline hover:text-black hover:underline mr-3 md:mr-5">Night Swim</a>
            <a href="#" class="text-grey-dark no-underline hover:text-black hover:underline mr-3 md:mr-5">Best Sellers</a>
          </div>
        </div>
      </div>
    </section>

    <section class="m-category-grid">
      <div class="container">
        <div class="flex flex-wrap">
          <product-teaser title="Something" price="310" image="images/day3@2x.png" />
        </div>
      </div>
    </section>
  </div>
</template>

<script>
  import ProductTeaser from '~/components/ProductTeaser.vue';
  
  export default {
    components: {
      ProductTeaser,
    },
    data() {
      return {
      }
    }
  }
</script>
