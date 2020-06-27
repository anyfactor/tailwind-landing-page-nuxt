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
    <div class="container mx-auto flex flex-wrap pt-4 pb-12">
      <teaser-column :rows="2" action="Visit" buttonBool path="https://www.notestem.com/">
        <template v-slot:headline
          >Notestem.com</template
        >
        <template v-slot:content
          >Blog about Orchestra and Band Instruments</template>
        <template v-slot:list>
          <div v-for="item in notestem" :key="item.id">
            <li>{{ item }}</li>
          </div>
        </template>
        <template v-slot:footer
          >
        </template>
      </teaser-column>
      <teaser-column :rows="2" action="Visit" buttonBool path="https://www.managechannel.com/">
        <template v-slot:headline
          >ManageChannel.com</template
        >
        <template v-slot:content
          >SAAS YouTube Channel Management services</template>
        <template v-slot:list>
          <div v-for="item in manage_channel" :key="item.id">
            <li>{{ item }}</li>
          </div>
        </template>
        <template v-slot:footer
          >
        </template>
      </teaser-column>

      <teaser-column :rows="2" action="Visit" buttonBool path="https://www.dailyidea.com/">
        <template v-slot:headline
          >DailyIdea.com
     </template>
        <template v-slot:content
          >Daily Idea noting and Idea based social platform</template>
        <template v-slot:list>
          <div v-for="item in daily_idea" :key="item.id">
            <li>{{ item }}</li>
          </div>
        </template>
        <template v-slot:footer
          >
        </template>
      </teaser-column>
      
      <teaser-column :rows="2" action="Visit" path="#">
        <template v-slot:headline
          >Service Hub</template
        >
        <template v-slot:content
          >Booking automobile service appointment service</template>
        <template v-slot:list>
          <div v-for="item in Social_hub" :key="item.id">
            <li>{{ item }}</li>
          </div>
        </template>
        <template v-slot:footer
          >
        </template>
      </teaser-column>

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
    <call-to-action />
</div>

</template>

<script>
import Hero from '@/components/Hero'
import CallToAction from '@/components/CallToAction'
import ContactButton from '@/components/ContactButton'
import FeatureRight from '@/components/FeatureRight'
import FeatureLeft from '@/components/FeatureLeft'
import TeaserColumn from '@/components/TeaserColumn'

export default {
    components: {
    hero: Hero,
    'call-to-action': CallToAction,
    'contact-button': ContactButton,
    'feature-right': FeatureRight,
    'feature-left': FeatureLeft,
    'teaser-column': TeaserColumn
    },
    data: function() {
        return {
        title: "Web Development",
        notestem: ['VueJs, Nuxt', 'Netlify & Netlify CMS', 'Github'],
        manage_channel: ['VueJs, Nuxt', 'Django REST', 'PostGreSQL', 'Github'],
        daily_idea: ['VueJs, Nuxt', 'SCSS', 'Template Modification', 'Github'],
        Social_hub: ['VueJs, Nuxt', 'Netlify & Netlify CMS',  'Laravel REST', 'PostGreSQL', 'Github'],
        technology: ['Stack: JAMstack (Javascript, API, Markup)', 'Preferred Role: Frontend Developer','Front End Framework: VueJs', 'Static Site Generator: NuxtJs', 'Frontend CSS Framework: BootstrapVue, Vuetify, Tailwind, SCSS', 'Static Site Deployment: Netlify, Github Pages',
                   'Content Management System: Netlify CMS, Nuxt Content', 'API: Firebase, Flask, FastAPI', 'Android, Cross Platform & Chrome Extension Development: Quasar','Backend: Python, Javascript', 'Database: SQLite3, PostGreSQL, JSON, Markdown']
        }
    }
}
</script>

<style>
</style>