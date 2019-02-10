<template>
  <header class="m-header">
    <div class="container mx-auto">
      <div class="flex items-center py-4 md:py-10">
        <div class="w-auto">
          <!-- Site Logo -->
          <logo />
        </div>
        <div class="w-auto ml-8 hidden md:block">
          <!-- Main Menu -->
          <nav class="flex flex-wrap">
            <nuxt-link to="/products" class="text-black no-underline hover:underline p-3 text-sm lg:text-base" >Swimwear</nuxt-link>
            <nuxt-link to="/lookbook" class="text-black no-underline hover:underline p-3 text-sm lg:text-base">Lookbook</nuxt-link>
            <nuxt-link to="/404" class="text-black no-underline hover:underline p-3 text-sm lg:text-base">Press</nuxt-link>
            <nuxt-link to="/about" class="text-black no-underline hover:underline p-3 text-sm lg:text-base">About</nuxt-link>
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
</template>

<script>
  import Logo from '~/components/Logo.vue'

  export default {
    components: {
      Logo
    },
    data() {
      return {
      }
    }
  }
</script>