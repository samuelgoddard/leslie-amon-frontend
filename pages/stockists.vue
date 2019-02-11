<template>
  <div>
    <section class="m-page-title w-full py-8 md:py-12">
      <div class="container">
        <div class="flex flex-wrap items-end">
          <div class="w-auto">
            <h1 class="text-black font-light text-3xl md:text-4xl lg:text-5xl leading-tight">Stockists</h1>
          </div>
        </div>
      </div>
    </section>

    <section class="mb-12 md:mb-24">
      <div class="container mb-12 md:mb-24">
        <div class="flex flex-wrap md:-mx-4">
          <div class="w-full md:w-1/2 lg:w-1/3 xl:w-1/4 md:px-4" v-for="stockist in stockists" :key="stockist.id">
            <div :class="stockist.classes" class="md:pr-6 lg:pr-8 xl:pr-12">
              <h2 class="font-thin text-xl md:text-2xl leading-tight mb-3">{{ stockist.title }}</h2>

              <p class="text-sm mb-3">{{ stockist.address }}</p>
              <a :href="'tel:' + stockist.tel" class="break-words text-black hover:text-grey-darker text-sm">{{ stockist.tel }}</a>
              <a href="" rel="noopener" target="_blank" class="break-words text-black hover:text-grey-darker text-sm">{{ stockist.website }}</a>
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
        stockists: [
          { 
            id: 1,
            title: 'Bergorf Goodman',
            address: ' 754 5th Ave, New York, NY 10019, États-Unis',
            tel: '+1 212-753-7300',
            website: 'https://www.bergdorfgoodman.com/',
            classes: 'mb-12 lg:mb-16 xl:mb-20'
          },{ 
            id: 2,
            title: 'Browns',
            address: '24-27 S Molton St  Mayfair, London W1K 5RD, Royaume-Uni',
            tel: '+44 20 3750 1241',
            website: 'https://www.brownsfashion.com/',
            classes: 'mb-12 lg:mb-16 xl:mb-20'
          },{ 
            id: 3,
            title: 'Bongenie Grieder',
            address: 'Rue du Marché 34, 1204 Genève, Suisse',
            tel: ' +41 22 818 11 11',
            website: 'https://www.bongenie-grieder.ch/',
            classes: 'mb-12 lg:mb-16 xl:mb-20'
          },{ 
            id: 4,
            title: 'Calarena',
            address: '​12 Rue du Général Leclerc, 20137 Porto-Vecchio Corsica',
            tel: '+33 4 95 21 88 39',
            website: 'http://calarena.com/',
            classes: 'mb-12 lg:mb-16 xl:mb-20'
          },{ 
            id: 5,
            title: 'Bergorf Goodman',
            address: ' 754 5th Ave, New York, NY 10019, États-Unis',
            tel: '+1 212-753-7300',
            website: 'https://www.bergdorfgoodman.com/',
            classes: 'mb-12 lg:mb-16 xl:mb-0'
          },{ 
            id: 6,
            title: 'Browns',
            address: '24-27 S Molton St  Mayfair, London W1K 5RD, Royaume-Uni',
            tel: '+44 20 3750 1241',
            website: 'https://www.brownsfashion.com/',
            classes: 'mb-12 lg:mb-0 xl:mb-0'
          },{ 
            id: 7,
            title: 'Bongenie Grieder',
            address: 'Rue du Marché 34, 1204 Genève, Suisse',
            tel: ' +41 22 818 11 11',
            website: 'https://www.bongenie-grieder.ch/',
            classes: 'mb-12 md:mb-0 lg:mb-0 xl:mb-0'
          },{ 
            id: 8,
            title: 'Calarena',
            address: '​12 Rue du Général Leclerc, 20137 Porto-Vecchio Corsica',
            tel: '+33 4 95 21 88 39',
            website: 'http://calarena.com/',
            classes: 'mb-12 md:mb-0 lg:mb-0 xl:mb-0'
          }
        ]
      }
    }
  }
</script>