<template>
  <div>
    <div v-if="modalOpen" class="m-modal fixed pin-t pin-r pin-b pin-l w-full min-h-full z-10">
      <div class="flex flex-wrap min-h-screen max-h-screen">
        <div @click="toggle()" class="hidden md:block md:w-1/2 lg:w-3/5 min-h-screen max-h-screen bg-black opacity-75">
        </div>
        <div class="w-full md:w-1/2 lg:w-2/5 min-h-screen max-h-screen bg-white">
          <div class="overflow-y-scroll w-full max-h-full block py-10 md:py-12 lg:py-16 px-6 md:px-12 lg:px-10">
            <div class="container">
              <div class="flex flex-wrap items-start">
                <div class="w-4/5 mb-4 md:mb-6">
                  <h2 class="font-thin text-2xl lg:text-3xl leading-tight">Delivery &amp; Returns</h2>
                </div>
                <div class="ml-auto text-right">
                  <button @click="toggle()" class="text-center flex ml-auto p-2 xl:p-3">
                    <svg viewPort="0 0 12 12" class="w-4 h-4 block" version="1.1"
                      xmlns="http://www.w3.org/2000/svg">
                      <line x1="1" y1="14" 
                        x2="14" y2="1" 
                        stroke="black" 
                        stroke-width="1"/>
                      <line x1="1" y1="1" 
                        x2="14" y2="14" 
                        stroke="black" 
                        stroke-width="1"/>
                    </svg>
                  </button>
                </div>
              </div>

              <h3 class="font-thin text-xl leading-tight mb-2">Switzerland</h3>
              <ul class="pl-4 ml-0 text-sm mb-4">
                <li>Priority Shipping, expect to deliver in 1-2 working days</li>
                <li>Price : 10 euros</li>
              </ul>

              <h3 class="font-thin text-xl leading-tight mb-2">Europe</h3>
              <ul class="pl-4 ml-0 text-sm mb-4 mb-4">
                <li>Priority Shipping, expect to deliver in 2-5 working days</li>
                <li>Price : 18 euros</li>
              </ul>

              <h3 class="font-thin text-xl leading-tight mb-2">Rest of the world</h3>
              <ul class="pl-4 ml-0 text-sm mb-4 mb-4">
                <li>Priority Shipping, expect to deliver in 3-7 working days
                <li>Price : 23 euros
                <li>Please consider the shipping address you provide, you should be attending <li>your address during normal business hours, as a signature may be required
                <li>Order are dispatched within 2 business days upon receiving your order
                <li>As soon as your order will be dispatched, you will receive your tracking number via email with an estimated arrival date</li>
                <li>For more info please contact our customer service : <a class="text-black hover:text-grey-dark" href="mailto:info.leslieamon@gmail.com">info.leslieamon@gmail.com</a></li>
              </ul>

              <h3 class="font-thin text-xl leading-tight mb-2">Returns</h3>
              <ul class="pl-4 ml-0 text-sm mb-4 mb-4">
                <li>We offer a 7 day returns policy</li>
                <li>We will gladly accept exchange on all items within 7 days upon reception</li>
                <li>Return are only accepted if the swimsuit is unworn, unwashed
                and if the sealed link and tags are still attached to the swimwear.</li>
                <li>The item needs to be return with it's original velvet pouch</li>
                <li>WE DONT OFFER EXCHANGE OR RETURN ON SALES PRODUCTS</li>
                <li>Shipping costs for refund are the responsibility of the customer.</li>
                <li>Please contact us at info.leslieamon@gmail.com to notify us,
                let us know which model you whish to exchange.</li>
                <li>Allow 3-5 days for processing upon reception
                Send Returns to: Leslie Amon, 9 place du Molard, 1204 Geneve, Switzerland</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
    <section class="m-product-overview mb-12 md:mb-24">
      <div class="container">
        <div class="flex flex-wrap items-center md:-mx-5">
          <div class="w-full md:w-3/5 md:px-5">
            <div class="flex flex-wrap items-center md:-mx-5">
              <div class="hidden md:block w-fill md:w-1/5 md:px-5">
                <div class="lg:pr-6">
                  <a href="#" class="no-underline block">
                    <img src="/../images/product-single@2x.png" alt="Amanda" class="w-full block mb-6" />
                  </a>
                  <a href="#" class="no-underline block opacity-25 hover:opacity-100 transition">
                    <img src="/../images/product-single@2x.png" alt="Amanda" class="w-full block mb-6" />
                  </a>
                  <a href="#" class="no-underline block opacity-25 hover:opacity-100 transition">
                    <img src="/../images/product-single@2x.png" alt="Amanda" class="w-full block mb-6" />
                  </a>
                  <a href="#" class="no-underline block opacity-25 hover:opacity-100 transition">
                    <img src="/../images/product-single@2x.png" alt="Amanda" class="w-full block mb-6" />
                  </a>
                </div>
              </div>
              <div class="w-full md:w-4/5 md:px-5 container--bleed--no-pad mb-6">
                <div class="lg:pr-12">
                  <img src="/../images/product-single@2x.png" alt="Amanda" class="w-full block " />
                </div>
              </div>
            </div>
          </div>
          <div class="w-full md:w-2/5 md:px-5">
            <div class="lg:pl-8">
              <span class="text-grey-dark text-sm mb-0">Swimwear / Bikini</span>
              <h2 class="text-3xl md:text-4xl lg:text-5xl font-thin leading-tight mb-5">Maryline</h2>

              <div class="mb-5">
                <span class="text-xl text-black line-through">310&euro;</span>
                <span class="text-xl text-red ml-2">124&euro;</span>
              </div>

              <p class="text-sm mb-6">A two piece swimsuit with ruffle made with the finest Italian fabric and the best French savoir faire.</p>

              <a href="#more-information" class="text-black hover:text-grey-dark text-sm inline-block mb-8">More information</a>

              <div class="flex flex-wrap -mx-3 mb-5">
                <div class="w-1/2 px-3">
                  <div class="inline-block relative w-full group">
                    <select class="block appearance-none w-full bg-white border border-black py-3 px-6 no-underline text-black hover:text-grey-dark text-center hover:bg-black hover:text-white transition rounded-none">
                      <option>Size</option>
                      <option>Small</option>
                      <option>Medium</option>
                      <option>Large</option>
                      <option>XLarge</option>
                    </select>
                    <div class="pointer-events-none absolute pin-y pin-r flex items-center px-2 text-black group-hover:text-white">
                      <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
                    </div>
                  </div>
                </div>
                <div class="w-1/2 px-3">
                  <div class="inline-block relative w-full group">
                    <select class="block appearance-none w-full bg-white border border-black py-3 px-6 no-underline text-black hover:text-grey-dark text-center hover:bg-black hover:text-white transition rounded-none">
                      <option>Colour</option>
                      <option>Black</option>
                      <option>White</option>
                      <option>Gold</option>
                    </select>
                    <div class="pointer-events-none absolute pin-y pin-r flex items-center px-2 text-black group-hover:text-white">
                      <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
                    </div>
                  </div>
                </div>
              </div>

              <a href="#" class="w-full block bg-black text-white border border-black text-center no-underline py-3 px-6 mb-10">Add to cart</a>

              <button @click="toggle()" class="text-black hover:text-grey-dark text-sm mr-5">Size guide</button>
              <button @click="toggle()" class="text-black hover:text-grey-dark text-sm mr-5">Delivery &amp; returns</button>
              <button @click="toggle()" class="text-black hover:text-grey-dark text-sm mr-5">Garment care</button>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="more-information" class="mb-12 md:mb-24">
      <div class="container mb-12 md:mb-24">
        <div class="flex flex-wrap justify-center">
          <div class="w-full lg:w-5/6">
            <div class="flex flex-wrap items-center md:-mx-5 md:flex-row-reverse">
              <div class="w-full md:w-3/5 lg:w-2/3 md:px-5 container--bleed--no-pad mb-12 md:mb-0">
                <img src="/../images/product-single2@2x.png" alt="Product Image" class="w-full block" />
              </div>

              <div class="w-full md:w-2/5 lg:w-1/3 md:px-5 mb-5 md:mb-0">
                <div class="lg:pr-6">
                  <h2 class="text-2xl md:text-3xl lg:text-4xl mb-5 font-light leading-tight">More information</h2>
                  <p class="text-sm mb-5">A belted one piece swim with contrast mat and shiny fabric. The swim can be worn with or without the strass buckle belt.</p>
                    
                  <p class="text-sm">This Swim has been design to be worn from day to night ; Swiming, Dining, and Lounging. Wear your swim as a bodysuit with a top, paired with a skirt or with a high waisted short.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Latest Feed - Product Grid -->
    <section class="m-feed mb-12 md:mb-24">
      <div class="container">
        <!-- Latest Feed - Title + Link -->
        <div class="flex flex-wrap items-end mb-4 md:mb-6">
          <div class="w-auto">
            <h2 class="font-light">Related products</h2>
          </div>
          <div class="w-auto ml-auto">
            <nuxt-link to="/products/" class="text-black text-sm hover:text-grey-dark">View all</nuxt-link>
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
        modalOpen: false,
        fakeActive: 'active-exact',
        products: [
          { 
            id: 1,
            title: 'Maryline',
            price: '310',
            image: '/../images/product1@2x.png'
          },{ 
            id: 2,
            title: 'Sacha',
            price: '310',
            image: '/../images/lame3@2x.png'
          },{ 
            id: 3,
            title: 'Tamini',
            price: '310',
            image: '/../images/stripes2@2x.png'
          },{ 
            id: 4,
            title: 'Kirsten',
            price: '310',
            image: '/../images/day3@2x.png'
          }
        ]
      }
    },
    methods: {
      toggle: function(){
        this.modalOpen = !this.modalOpen
      }
    }
  }
</script>