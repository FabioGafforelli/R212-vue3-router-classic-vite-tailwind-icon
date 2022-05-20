<script>
import card from "../components/Card.vue"
import header1 from "../components/Header.vue"
import footer1 from "../components/Footer.vue"
import flechedown from "../components/icones/Flechedown.vue"
import loupe from "../components/icones/loupe.vue"


export default {
    name:"App",
    components: { card, header1, footer1, flechedown, loupe },
}
</script>

<template class="bg-indigo-25">
    <header1 />
    <div class="bg-indigo-25">



<div class="lg:flex lg:justify-between">
      <h1 class="m-4 mt-14 text-4xl font-bold text-center">Search properties to rent</h1>

      <div class="mt-14 mx-6 px-2 py-1 border-2 border-indigo-100 rounded-lg flex justify-between bg-white lg:flex-1 py-1 ml-32">
          <p class="text-gray-900 font-medium text-left lg:">Search with Search Bar</p>

          <flechedown class="p-1 my-1 bg-indigo-100 rounded-xl lg:p-2  "/>
      </div>
    </div>

    <div class="mt-10 mx-6 flex justify-between bg-white rounded-lg">
      <p class=" px-2 py-4 text-gray-500 font-medium">Search location</p>

      <loupe class="bg-indigo-500 m-2 p-3"/>
    </div>




    <div class="grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(343px,1fr))]">

        <card class="p-4" 
        image="/images-maison/maison1.jpg" 
        titre="Beverly Springfield"
        lieu="2821 Lake Sevilla, Palm Harbor, TX"
        nbrSDB="2"/>

        <card class="p-4"
        image="/images-maison/maison2.jpg"
        titre="Palm Harbor"
        lieu="2699 Green Valley, Highland Lake"
        :price="2095"
        nbrSDB="2"/>

        <card class="p-4"
        image="/images-maison/maison3.jpg"
        titre="Faulkner Ave" 
        lieu="909 Woodland St, Michigan, IN"
        :price="4550" 
        nbrSDB="3"/>

        <card class="p-4"
        :favoris="true"
        image="/images-maison/maison4.jpg"
        titre="St. Christal"
        lieu="210 US Highway, HighlandLake, FL"
        :price="4650"
        nbrSDB="2"/>

        <card class="p-4"
        image="/images-maison/maison5.jpg"
        titre="Cover Red"
        lieu="243 CurlewRoad, PalmHarbor, TX"
        :price="3100"
        nbrSDB="2"/>

        <card class="p-4"
        :favoris="true" 
        image="/images-maison/maison6.jpg"
        titre="Tarpon Bay" 
        lieu="103 Lake Shores, Michigan, IN"
        :price="4800" 
        nbrSDB="3"/>

    </div>
    </div>
    <footer1 />

</template>