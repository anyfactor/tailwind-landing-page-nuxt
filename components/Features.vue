<template>
  <section class="bg-white py-8">
    <div class="container max-w-5xl mx-auto m-8">
      <h1
        class="w-full my-2 text-5xl font-bold leading-tight text-center text-gray-800"
      >
        Languages
      </h1>
      <div class="w-full mb-4">
        <div
          class="h-1 mx-auto gradient w-64 opacity-25 my-0 py-0 rounded-t"
        ></div>
      </div>
      <feature-right
        headline="Python"
        content="I have been a professional python developer for years now. While some take python as a tool or merely a programming language, my use case of python derives from the passion I feel for it."
        footer="That is why I have explored and learned all the extensive applications of python.""
      >
        <img src="~assets/img/travel-booking.svg" alt slot="svg" />
      </feature-right>
      <feature-left
        headline="VueJs"
        content="It is convenient, easy to use and can be progressively affordable. With many options, VueJs is the right, light, and the most powerful option for building websites that deliver."
        footer="Like Python, VueJs in my heart has a special place."
      >
        <img src="~assets/img/connected-world.svg" alt slot="svg" />
      </feature-left>
    </div>
  </section>
</template>

<script>
import FeatureRight from '@/components/FeatureRight'
import FeatureLeft from '@/components/FeatureLeft'

export default {
  name: 'Features',
  components: {
    'feature-right': FeatureRight,
    'feature-left': FeatureLeft
  }
}
</script>
