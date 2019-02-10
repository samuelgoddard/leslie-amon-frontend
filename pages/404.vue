<template>
  <div>
    <section class="mb-12 md:mb-24">
      <div class="container mb-12 md:mb-24">
        <div class="flex flex-wrap justify-center">
          <div class="w-full">
            <div class="flex flex-wrap items-center md:-mx-5">
              <div class="w-full md:w-1/2 md:px-5 container--bleed--no-pad mb-12 md:mb-0">
                <img src="images/about@2x.png" alt="About Leslie Amon" class="w-full block" />
              </div>

              <div class="w-full md:w-1/2 md:px-5 mb-5 md:mb-0">
                <div class="md:px-6 lg:px-24">
                  <div class="mb-5">
                    <h2 class="font-thin text-3xl xl:text-4xl mb-3 md:mb-5">Page not found</h2> 
                    <p class="text-base lg:text-lg xl:text-xl text-black mb-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Blanditiis earum possimus nostrum deserunt, delectus distinctio.</p>

                    <p class="text-sm">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptas natus illo harum non soluta dolor possimus rem quas voluptatum! Possimus.</p>
                  </div>

                  <h3 class="font-thin text-xl mb-3">Navigate</h3>
                  <nav>
                    <nuxt-link to="/products" class="inline-block mr-3 text-black no-underline hover:underline text-sm" >Swimwear</nuxt-link>
                    <nuxt-link to="/lookbook" class="inline-block mr-3 text-black no-underline hover:underline text-sm">Lookbook</nuxt-link>
                    <nuxt-link to="/404" class="inline-block mr-3 text-black no-underline hover:underline text-sm">Press</nuxt-link>
                    <nuxt-link to="/about" class="inline-block mr-3 text-black no-underline hover:underline text-sm">About</nuxt-link>
                  </nav>
                </div>
              </div>
            </div>
          </div>
        </div>
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
      }
    }
  }
</script>