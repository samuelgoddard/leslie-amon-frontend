<template>
  <div>
    <!-- Hero Banner -->
    <section class="m-hero w-full flex items-center py-8 md:py-16 lg:py-32 mb-10 md:mb-12" style="background: url(/images/100@2x.png) no-repeat center center #ECADAD; background-size: cover;">

      <div class="container py-32">
        <div class="w-full text-center">
          <!-- Hero Banner -- CTA Link Text -->
          <nuxt-link to="/category" class="group no-underline inline-block">
            <h1 class="text-white font-light text-xl md:text-2xl lg:text-3xl">Spring Summer 2019</h1>
            <span class="text-white inline-block p-2 border transition border-transparent group-hover:border-white mt-2">Shop the range</span>
          </nuxt-link>
        </div>
      </div>
    </section>

    <!-- Latest Feed -->
    <section class="m-feed mb-12 md:mb-24">
      <div class="container">
        <!-- Latest Feed - Title + Link -->
        <div class="flex flex-wrap items-end mb-4 md:mb-6">
          <div class="w-auto">
            <h2 class="font-light">New Styles</h2>
          </div>
          <div class="w-auto ml-auto">
            <a href="#" class="text-black text-sm">View all</a>
          </div>
        </div>
        <!-- Latest Feed - Product Grid -->
        <div class="flex flex-wrap -mx-4 lg:-mx-7">
          <div class="w-1/2 md:w-1/4 px-4 lg:px-7 mb-5 md:mb-0" v-for="product in products" v-bind:key="product.id">
            <!-- Latest Feed - Product Grid - Teaser -->
            <product-teaser :title="product.title" :price="product.price" :image="product.image" />
          </div>
        </div>
      </div>
    </section>

    <!-- Show Your Stripes Featured Teaser -->
    <section class="mb-12 md:mb-24">
      <div class="container mb-12 md:mb-24">
        <div class="flex flex-wrap justify-center">
          <div class="w-full md:w-5/6">
            <div class="flex flex-wrap items-center md:-mx-5 md:flex-row-reverse">
              <div class="w-full md:w-2/3 md:px-5 container--bleed--no-pad mb-12 md:mb-0">
                <img src="images/amanda@2x.png" alt="Product Image" class="w-full block" />
              </div>

              <div class="w-full md:w-1/3 md:px-5 mb-5 md:mb-0">
                <h2 class="text-5xl md:text-3xl lg:text-5xl mb-5 font-light leading-tight">Show Your Stripes</h2>
                <p class="text-sm mb-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eos officia quas aperiam provident, veritatis delectus. Harum itaque tempore labore? Quas cupiditate.</p>

                <a href="#" class="text-black text-sm">Shop now</a>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="container">
        <div class="flex flex-wrap items-center mb-12 md:mb-24 justify-center">
          <div class="w-auto md:w-3/5 container--bleed--no-pad mb-16 md:mb-0">
            <img src="images/stripes1@2x.png" alt="Product Image" class="w-full block" />
          </div>
          <div class="w-4/5 md:w-1/4 md:ml-auto">
            <product-teaser title="Something" price="310" image="images/stripes2@2x.png" />
          </div>
        </div>
      </div>
    </section>

    <!-- From Day To Night Featured Teaser -->
    <section class="mb-12 md:mb-24">
      <div class="container mb-12 md:mb-24">
        <div class="flex flex-wrap justify-center">
          <div class="w-full md:w-5/6">
            <div class="flex flex-wrap items-center md:-mx-5">
              <div class="w-full md:w-2/3 md:px-5 container--bleed--no-pad mb-12 md:mb-0">
                <img src="images/day1@2x.png" alt="Product Image" class="w-full block" />
              </div>

              <div class="w-full md:w-1/3 md:px-5 mb-5 md:mb-0">
                <h2 class="text-5xl md:text-3xl lg:text-5xl mb-5 font-light leading-tight">From day to night</h2>
                <p class="text-sm mb-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eos officia quas aperiam provident, veritatis delectus. Harum itaque tempore labore? Quas cupiditate.</p>

                <a href="#" class="text-black text-sm">Shop now</a>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="container">
        <div class="flex flex-wrap items-center mb-12 md:mb-24 justify-center md:flex-row-reverse">
          <div class="w-auto md:w-3/5 container--bleed--no-pad mb-16 md:mb-0 md:ml-auto">
            <img src="images/day2@2x.png" alt="Product Image" class="w-full block" />
          </div>
          <div class="w-4/5 md:w-1/4">
            <product-teaser title="Something" price="310" image="images/day3@2x.png" />
          </div>
        </div>
      </div>
    </section>

    <!-- Lame Featured Teaser -->
    <section class="mb-12 md:mb-24">
      <div class="container mb-12 md:mb-24">
        <div class="flex flex-wrap justify-center">
          <div class="w-full md:w-5/6">
            <div class="flex flex-wrap items-center md:-mx-5 md:flex-row-reverse">
              <div class="w-full md:w-2/3 md:px-5 container--bleed--no-pad mb-12 md:mb-0">
                <img src="images/lame1@2x.png" alt="Product Image" class="w-full block" />
              </div>

              <div class="w-full md:w-1/3 md:px-5 mb-5 md:mb-0">
                <h2 class="text-5xl md:text-3xl lg:text-5xl mb-5 font-light leading-tight">Lame</h2>
                <p class="text-sm mb-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eos officia quas aperiam provident, veritatis delectus. Harum itaque tempore labore? Quas cupiditate.</p>

                <a href="#" class="text-black text-sm">Shop now</a>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="container">
        <div class="flex flex-wrap items-center mb-12 md:mb-24 justify-center">
          <div class="w-auto md:w-3/5 container--bleed--no-pad mb-16 md:mb-0">
            <img src="images/lame2@2x.png" alt="Product Image" class="w-full block" />
          </div>
          <div class="w-4/5 md:w-1/4 md:ml-auto">
            <product-teaser title="Something" price="310" image="images/lame3@2x.png" />
          </div>
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
        products: [
          { 
            id: 1,
            title: 'Maryline',
            price: '310',
            image: 'images/product1@2x.png'
          },{ 
            id: 2,
            title: 'Sacha',
            price: '310',
            image: 'images/product1@2x.png'
          },{ 
            id: 3,
            title: 'Tamini',
            price: '310',
            image: 'images/product1@2x.png'
          },{ 
            id: 3,
            title: 'Kirsten',
            price: '310',
            image: 'images/product1@2x.png'
          }
        ]
      }
    }
  }
</script>
