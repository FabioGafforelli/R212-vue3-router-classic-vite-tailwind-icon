<script>
import Logo from './icones/Logo.vue'
import Navigation from './icones/Navbar.vue'
import Flechedown from './icones/Flechedown.vue'
import Bouton from ".//icones/Bouton.vue";

export default {
    components: { Logo, Navigation, Flechedown, Bouton },
}

</script>

<template>
    <header class=" border-b-2 border-indigo-100 bg-white">
        <div class=" flex justify-between m-6  ">
            <Logo/>
            <Navigation class="xl:hidden"/>
          <div class="hidden xl:flex items-center overflow-hidden relative gap-2.5">
    <div class="flex overflow-hidden gap-10">
      <p class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-gray-900">Rent</p>
      <p class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-gray-900">Buy</p>
      <p class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-gray-900">Sell</p>
      <p class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-gray-900">Manage Property</p>
    </div>
    <Flechedown/>
    <div class="flex justify-start items-center overflow-hidden gap-10">
      <p class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-gray-900">Resources</p>
    </div>
    <flechedown/>
  </div>
  <Bouton/>
  </div>
    </header>

</template>
