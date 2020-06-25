<template>
  <div class="flex flex-wrap">
    <div class="w-5/6 sm:w-1/2 p-6">
      <h3 class="text-3xl text-left text-gray-800 font-bold leading-none mb-3">
        {{ headline }}
      </h3>
      <p class="text-gray-600">
        {{ content }}
      </p>
      <ul class="my-2 list-disc mx-auto list-inside">
        <li v-for="item in list" :key="item.id" class="text-gray-600">
          {{ item }}
        </li>
      </ul>
      <p class="text-gray-600 mb-4">
        {{ footer }}
      </p>
     <nuxt-link :to="path">
      <button
        class="mx-auto lg:mx-0 hover:underline gradient text-white font-bold rounded-full py-4 px-8 shadow-lg"
      >
        {{ buttonName }}
      </button>
    </nuxt-link>
    </div>
    <div class="w-full sm:w-1/2 p-6">
      <slot name="svg" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'FeatureRight',
  props: {
    headline: {
      type: String,
      required: false
    },
    content: {
      type: String,
      required: false
    },
    list: {
      type: Array,
      required: false
    },
    footer: {
      type: String,
      required: false
    },
    path: {
      type: String,
      required: false
    },
    buttonName: {
      type: String,
      required: false
    }
  }
}
</script>
