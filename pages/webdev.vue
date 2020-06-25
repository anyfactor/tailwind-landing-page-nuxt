<template>
<div>
    <hero />
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
      <feature-left
        headline="Notestem.com"
        content="I will help you create a beautiful, lightweight and user-focused website that is easy to operate and close as free to maintain."
        :list="notestem"
        footer="Whatever it is send me an email and we will make dreams into reality."
        path="https://www.notestem.com/"
        buttonName="Visit"
      >
   
      <img src="~/assets/img/web dev/notestem.png" alt slot="svg" />
      </feature-left>


         <div>
            <h1 class="w-full my-1 text-3xl font-bold leading-tight text-left text-gray-800">
      Technology & Tool
    </h1>



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
    <call-to-action />
</div>

</template>

<script>
import Hero from '@/components/Hero'
import CallToAction from '@/components/CallToAction'
import ContactButton from '@/components/ContactButton'
import FeatureRight from '@/components/FeatureRight'
import FeatureLeft from '@/components/FeatureLeft'

export default {
    components: {
    hero: Hero,
    'call-to-action': CallToAction,
    'contact-button': ContactButton,
    'feature-right': FeatureRight,
    'feature-left': FeatureLeft
    },
    data: function() {
        return {
        title: "Web Scraping",
        notestem: ['VueJs, Nuxt', 'Netlify & Netlify CMS', 'Github'],
        technology: ['Python', 'Selenium, Requests-HTML', 'Requests, URLLib, Beautiful Soup 4', 'Regex', 'Pandas, Numpy', 'Microsoft Excel, Google Sheets', 'SQL']
        }
    }
}
</script>

<style>
</style>