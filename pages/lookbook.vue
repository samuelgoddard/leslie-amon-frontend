<template>
  <div>
    <!-- Page Title -->
    <section class="m-page-title w-full py-8 md:py-12">
      <div class="container">
        <div class="flex flex-wrap items-end">
          <div class="w-auto">
            <h1 class="text-black font-light text-3xl md:text-4xl lg:text-5xl leading-tight">High Summer 2019</h1>
          </div>
          <div class="w-auto ml-auto">
            <a href="#" class="text-black hover:text-grey-dark">Preorder</a>
          </div>
        </div>
      </div>
    </section>

    <section class="m-lookbook-carousel mb-12 md:mb-24">
      <!-- Category Feed -->
      <div class="sm:overflow-x-scroll sm:whitespace-no-wrap mx-4 sm:mx-0 pb-1 sm:mb-2">
          <!-- Latest Feed - Product Grid - Teaser -->
          <img v-for="product in products" :key="product.id" :src="product.image" :alt="product.title" class="h-auto mb-4 sm:mb-0 sm:h-82 md:h-124 lg:h-164 block sm:inline-block sm:mx-3"
          v-bind:class="{ 'sm:ml-0': product.first, 'sm:mr-0': product.last }" />
      </div>
      <div class="container hidden sm:block">
        <p>01/29</p>
      </div>
    </section>
  </div>
</template>

<script>  
  export default {
    components: {
    },
    data() {
      return {
        products: [
          { 
            id: 1,
            title: 'Maryline',
            price: '310',
            image: '/../images/product-teasers/1@2x.jpg',
            first: true
          },{ 
            id: 2,
            title: 'Sacha',
            price: '310',
            image: '/../images/day1@2x.jpg'
          },{ 
            id: 3,
            title: 'Tamini',
            price: '310',
            image: '/../images/product-teasers/1@2x.jpg'
          },{ 
            id: 4,
            title: 'Kirsten',
            price: '310',
            image: '/../images/day1@2x.jpg'
          },{ 
            id: 5,
            title: 'Amanda',
            price: '310',
            image: '/../images/product-teasers/1@2x.jpg'
          },{ 
            id: 6,
            title: 'Amanda',
            price: '310',
            image: '/../images/day1@2x.jpg'
          },{ 
            id: 7,
            title: 'Sarah',
            price: '310',
            image: '/../images/product-teasers/1@2x.jpg'
          },{ 
            id: 8,
            title: 'Tami',
            price: '310',
            image: '/../images/day1@2x.jpg',
            last: true
          }
        ]
      }
    }
  }
</script>
