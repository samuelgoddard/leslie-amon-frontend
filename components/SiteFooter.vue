<template>
  <footer class="m-footer sm:mb-8">
    <div class="container">
      <!-- <div class="w-full md:w-2/5 bg-grey-lightest py-4 sm:p-6 container--bleed mb-6 md:mb-0">
        <h3 class="text-xl font-light mb-4">Stay updated</h3>

        <form class="w-full mb-5">
          <div class="flex items-end">
            <input class="appearance-none rounded-none bg-white border-b border-black w-full text-black py-2 px-4 focus:outline-none text-sm focus:border-transparent transition" type="email" placeholder="Enter Email..." aria-label="Email Address" required>
            <input class="appearance-none rounded-none bg-white text-sm text-black hover:bg-black hover:text-white focus:bg-black focus:text-white py-2 px-4 border-b border-black" type="submit" value="Send" />
          </div>
        </form>

        <a href="#" class="text-sm text-black">Instagram</a>
        <a href="#" class="text-sm text-black ml-2">Facebook</a>
      </div> -->

      <div class="flex flex-wrap">
        <div class="w-1/2 md:w-1/4 mb-12 md:mb-0">
          <a href="#" class="block text-black text-sm no-underline hover:underline mb-3 md:mb-4 pr-2">Newsletter</a>
          <a href="#" class="block text-black text-sm no-underline hover:underline mb-3 md:mb-4 pr-2">Instagram</a>
          <a href="#" class="block text-black text-sm no-underline hover:underline mb-3 md:mb-4 pr-2">Facebook</a>
        </div>
        <div class="w-1/2 md:w-1/4 mb-12 md:mb-0">
          <a href="#" class="block text-black text-sm no-underline hover:underline mb-3 md:mb-4 pr-2">Contact</a>
          <a href="#" class="block text-black text-sm no-underline hover:underline mb-3 md:mb-4 pr-2">Stockists</a>
          <a href="#" class="block text-black text-sm no-underline hover:underline mb-3 md:mb-4 pr-2">Press</a>
        </div>
        <div class="w-1/2 md:w-1/4 mb-12 md:mb-0">
          <a href="#" class="block text-black text-sm no-underline hover:underline mb-3 md:mb-4 pr-2">Taxes &amp; Duties</a>
          <a href="#" class="block text-black text-sm no-underline hover:underline mb-3 md:mb-4 pr-2">Shipping Information</a>
          <a href="#" class="block text-black text-sm no-underline hover:underline mb-3 md:mb-4 pr-2">Returns</a>
        </div>
        <div class="w-1/2 md:w-1/4 mb-12 md:mb-0">
          <a href="#" class="block text-black text-sm no-underline hover:underline mb-3 md:mb-4 pr-2">Terms &amp; Conditions</a>
          <a href="#" class="block text-black text-sm no-underline hover:underline mb-3 md:mb-4 pr-2">Privacy</a>
        </div>
      </div>

      <!-- <div class="w-full md:w-3/5">
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
      </div> -->
    </div>
  </footer>  
</template>

<script>
  export default {
    components: {
    },
    data() {
      return {
        footerLinks: [
          { 
            id: 1,
            title: 'Newsletter',
            link: '#',
          },{ 
            id: 2,
            title: 'Contact',
            link: '#',
          },{ 
            id: 3,
            title: 'Taxes & Duties',
            link: '#',
          },{ 
            id: 4,
            title: 'Terms & Conditions',
            link: '#',
          },{ 
            id: 5,
            title: 'Instagram',
            link: '#',
          },{ 
            id: 6,
            title: 'Stockists',
            link: '#',
          },{ 
            id: 7,
            title: 'Shipping Information',
            link: '#',
          },{ 
            id: 8,
            title: 'Privacy',
            link: '#',
          },{ 
            id: 9,
            title: 'Facebook',
            link: '#',
          },{ 
            id: 10,
            title: 'Press',
            link: '#',
          },{ 
            id: 11,
            title: 'Returns',
            link: '#',
          }
        ]
      }
    }
  }
</script>