<template>
  <div>
    <!-- Page Title -->
    <section class="m-page-title w-full py-8 md:py-12 mb-4">
      <div class="container">
        <div class="w-full">
          <h1 class="text-black font-light text-3xl md:text-4xl lg:text-5xl mb-3 leading-tight">Swimwear</h1>
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
        <!-- Category Feed -->
        <div class="flex flex-wrap -mx-4">
          <div class="w-1/2 md:w-1/4 px-4 mb-5 md:mb-8 lg:mb-12 xl:mb-16" v-for="product in products" v-bind:key="product.id">
            <!-- Latest Feed - Product Grid - Teaser -->
            <product-teaser :title="product.title" :price="product.price" :image="product.image" />
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
            image: '/../images/product-teasers/1@2x.jpg'
          },{ 
            id: 2,
            title: 'Sacha',
            price: '310',
            image: '/../images/product-teasers/2@2x.jpg'
          },{ 
            id: 3,
            title: 'Tamini',
            price: '310',
            image: '/../images/product-teasers/3@2x.jpg'
          },{ 
            id: 4,
            title: 'Kirsten',
            price: '310',
            image: '/../images/product-teasers/4@2x.jpg'
          },{ 
            id: 5,
            title: 'Amanda',
            price: '310',
            image: '/../images/product-teasers/5@2x.jpg'
          },{ 
            id: 6,
            title: 'Amanda',
            price: '310',
            image: '/../images/product-teasers/6@2x.jpg'
          },{ 
            id: 7,
            title: 'Sarah',
            price: '310',
            image: '/../images/product-teasers/7@2x.jpg'
          },{ 
            id: 8,
            title: 'Tami',
            price: '310',
            image: '/../images/product-teasers/8@2x.jpg'
          },{ 
            id: 9,
            title: 'Maryline',
            price: '310',
            image: '/../images/product-teasers/1@2x.jpg'
          },{ 
            id: 10,
            title: 'Sacha',
            price: '310',
            image: '/../images/product-teasers/2@2x.jpg'
          },{ 
            id: 11,
            title: 'Tamini',
            price: '310',
            image: '/../images/product-teasers/3@2x.jpg'
          },{ 
            id: 12,
            title: 'Kirsten',
            price: '310',
            image: '/../images/product-teasers/4@2x.jpg'
          }
        ]
      }
    }
  }
</script>
