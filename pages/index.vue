<template>
  <div>
    <header class="m-header">
      <div class="container mx-auto">
        <div class="flex items-center py-5 md:py-10">
          <div class="w-auto">
            <!-- Site Logo -->
            <logo />
          </div>
          <div class="w-auto ml-8 hidden md:block">
            <!-- Main Menu -->
            <nav class="flex flex-wrap">
              <a class="text-black no-underline hover:underline p-3 text-sm lg:text-base" href="#">Swimwear</a>
              <a class="text-black no-underline hover:underline p-3 text-sm lg:text-base" href="#">Lookbook</a>
              <a class="text-black no-underline hover:underline p-3 text-sm lg:text-base" href="#">Press</a>
              <a class="text-black no-underline hover:underline p-3 text-sm lg:text-base" href="#">About</a>
            </nav>
          </div>
          <div class="w-auto ml-auto">
            <!-- Right Meta Menu -->
            <nav class="flex flex-wrap">
              <a class="text-black no-underline hover:underline p-3 text-sm lg:text-base" href="#">Search</a>
              <a class="text-black no-underline hover:underline p-3 text-sm lg:text-base" href="#">Cart</a>
              <!-- Burger Menu Icon Toggle -->
              <button class="flex md:hidden items-center rounded text-black p-3 pr-0 hover:text-pink">
                <svg class="fill-current h-5 w-5" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
              </button>
            </nav>
          </div>
        </div>
      </div>
    </header>

    <!-- Hero Banner -->
    <section class="m-hero bg-pink w-full flex items-center py-8 md:py-16 lg:py-32 mb-10 md:mb-12">
      <div class="container py-32">
        <div class="w-full text-center">
          <!-- Hero Banner -- CTA Link Text -->
          <a href="#" class="group no-underline inline-block">
            <h1 class="text-white font-light text-3xl">Spring Summer 2019</h1>
            <span class="text-white inline-block p-2 border transition border-transparent group-hover:border-white group-hover:mt-2">Shop the range</span>
          </a>
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
        <div class="flex flex-wrap -mx-4 lg:-mx-6">
          <div class="w-1/2 md:w-1/4 px-4 lg:px-6 mb-5 md:mb-0" v-for="product in products" v-bind:key="product.id">
            <!-- Latest Feed - Product Grid - Teaser -->
            <a href="#" class="m-product-teaser no-underline text-black hover:underline">
              <img :src="product.image" alt="Product Image" class="w-full mb-2" />
              <span class="block text-black text-lg">{{ product.title }}</span>
              <span class="block text-grey-dark text-sm">{{ product.price }}&euro;</span>
            </a>
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
                <img src="https://via.placeholder.com/720x480/F6F6F6" alt="Product Image" class="w-full" />
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
            <img src="https://via.placeholder.com/720x540/F6F6F6" alt="Product Image" class="w-full" />
          </div>
          <div class="w-4/5 md:w-1/4 md:ml-auto">
            <a href="#" class="m-product-teaser no-underline text-black hover:underline">
              <img src="https://via.placeholder.com/550x750/F6F6F6" alt="Product Image" class="w-full mb-2" />
              <span class="block text-black text-lg">Something</span>
              <span class="block text-grey-dark text-sm">310&euro;</span>
            </a>
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
                <img src="https://via.placeholder.com/720x480/F6F6F6" alt="Product Image" class="w-full" />
              </div>

              <div class="w-full md:w-1/3 md:px-5 mb-5 md:mb-0">
                <h2 class="text-5xl md:text-3xl lg:text-5xl mb-5 font-light leading-tight">From Day To Night</h2>
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
            <img src="https://via.placeholder.com/720x540/F6F6F6" alt="Product Image" class="w-full" />
          </div>
          <div class="w-4/5 md:w-1/4">
            <a href="#" class="m-product-teaser no-underline text-black hover:underline">
              <img src="https://via.placeholder.com/550x750/F6F6F6" alt="Product Image" class="w-full mb-2" />
              <span class="block text-black text-lg">Something</span>
              <span class="block text-grey-dark text-sm">310&euro;</span>
            </a>
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
                <img src="https://via.placeholder.com/720x480/F6F6F6" alt="Product Image" class="w-full" />
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
            <img src="https://via.placeholder.com/720x540/F6F6F6" alt="Product Image" class="w-full" />
          </div>
          <div class="w-4/5 md:w-1/4 md:ml-auto">
            <a href="#" class="m-product-teaser no-underline text-black hover:underline">
              <img src="https://via.placeholder.com/550x750/F6F6F6" alt="Product Image" class="w-full mb-2" />
              <span class="block text-black text-lg">Something</span>
              <span class="block text-grey-dark text-sm">310&euro;</span>
            </a>
          </div>
        </div>
      </div>
    </section>

    <!-- Site Footer -->
    <footer class="m-footer sm:mb-8">
      <div class="container">
        <div class="flex flex-wrap items-center">
          <div class="w-full md:w-2/5 bg-grey-lightest py-4 sm:p-6 container--bleed mb-6 md:mb-0">
            <h3 class="text-xl font-light mb-4">Stay updated</h3>

            <form class="w-full mb-5">
              <div class="flex items-center">
                <input class="appearance-none bg-white border-b border-black w-full text-black py-2 px-4 focus:outline-none text-sm focus:border-transparent transition" type="email" placeholder="Enter Email..." aria-label="Email Address" required>
                <input class="flex-no-shrink bg-white text-sm text-black hover:bg-black hover:text-white focus:bg-black focus:text-white py-2 px-4 border-b border-black" type="submit" value="Send" />
              </div>
            </form>

            <a href="#" class="text-sm text-black">Instagram</a>
            <a href="#" class="text-sm text-black ml-2">Facebook</a>
          </div>

          <div class="w-full md:w-3/5">
            <div class="flex flex-wrap md:pl-10">
              <div class="mb-8 sm:mb-0 w-1/2 sm:w-1/3">
                <div><a href="#" class="text-black text-sm no-underline hover:underline">Contact</a></div>
                <div><a href="#" class="text-black text-sm no-underline hover:underline">Stockists</a></div>
                <div><a href="#" class="text-black text-sm no-underline hover:underline">Press</a></div>
            </div>

              <div class="mb-8 sm:mb-0 w-1/2 sm:w-1/3">
                <div><a href="#" class="text-black text-sm no-underline hover:underline">Taxes &amp; Duties</a></div>
                <div><a href="#" class="text-black text-sm no-underline hover:underline">Shipping Information</a></div>
                <div><a href="#" class="text-black text-sm no-underline hover:underline">Returns</a></div>
            </div>

              <div class="mb-8 sm:mb-0 w-1/2 sm:w-1/3">
                <div><a href="#" class="text-black text-sm no-underline hover:underline">Terms &amp; Conditions</a></div>
                <div><a href="#" class="text-black text-sm no-underline hover:underline">Privacy</a></div>
            </div>
            </div>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  data() {
    return {
      products: [
        { 
          id: 1,
          title: 'Maryline',
          price: 310,
          image: 'https://via.placeholder.com/550x750/F6F6F6'
        },{ 
          id: 2,
          title: 'Sacha',
          price: 310,
          image: 'https://via.placeholder.com/550x750/F6F6F6'
        },{ 
          id: 3,
          title: 'Tamini',
          price: 310,
          image: 'https://via.placeholder.com/550x750/F6F6F6'
        },{ 
          id: 3,
          title: 'Kirsten',
          price: 310,
          image: 'https://via.placeholder.com/550x750/F6F6F6'
        }
      ]
    }
  }
}
</script>
