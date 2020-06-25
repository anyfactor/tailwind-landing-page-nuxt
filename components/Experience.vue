<template>
  <section class="bg-white py-8">
    <div class="container max-w-5xl mx-auto m-8">
      <h1
        class="w-full my-2 text-5xl font-bold leading-tight text-center text-gray-800"
      >
        {{ title }}
      </h1>
      <div class="w-full mb-4">
        <div
          class="h-1 mx-auto gradient w-64 opacity-25 my-0 py-0 rounded-t"
        ></div>
      </div>
    <h1 class="w-full my-1 text-3xl font-bold leading-tight text-left text-gray-800">
      Experience
    </h1>
    <div class="mx-auto font-bold leading-tight text-gray-700 m-10">
      <ul>
        <li v-for="item in items" :key="item.id" class="list-disc m-3">
          {{ item }}
        </li>
      </ul>
      </div>
      <div>
            <h1 class="w-full my-1 text-3xl font-bold leading-tight text-left text-gray-800">
      Technology & Tool
    </h1>
        <div class="mx-auto font-bold leading-tight text-gray-700 m-10">
      <ul>
        <li v-for="item in technology" :key="item.id" class="list-disc m-3">
          {{ item }}
        </li>
      </ul>
      </div>
    <nuxt-link to="/">
      <button
        class="mx-auto lg:mx-0 hover:underline gradient text-white font-bold rounded-full py-4 px-8 shadow-lg"
      >
        Go Back to Home?
      </button>
    </nuxt-link>
    <contact-button class="mx-auto lg:mx-0 hover:underline gradient text-white font-bold rounded-full py-4 px-8 shadow-lg">
    </contact-button>
      </div>
    </div>
  </section>
</template>

<script>

import ContactButton from '@/components/ContactButton'

export default {
  // props:{
  //   title: {
  //     type: String,
  //     required: false
  //   },
  //   items: {
  //     type: Array,
  //     required: false
  //   }
  // }
  components: {
    'contact-button': ContactButton
  },
  props: ['title', 'items', 'technology'],
}
</script>