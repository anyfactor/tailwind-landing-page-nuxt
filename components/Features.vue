<template>
  <section class="bg-white py-8">
    <div class="container max-w-5xl mx-auto">
      <h1
        class="w-full my-2 text-5xl font-bold leading-tight text-center text-gray-800"
      >
        Services
      </h1>
      <div class="w-full mb-4">
        <div
          class="h-1 mx-auto gradient w-64 opacity-25 my-0 py-0 rounded-t"
        ></div>
      </div>
      <feature-right
        headline="Automation & Bots"
        content="I can create scripts to automate your boring repetitive tasks. Whatever you can think of "
        :list="automation_list"
        footer="I can automate that. I will set up scripts using Remote Assistance and will provide detailed video instruction."
        path="/automation"
        buttonName="Portfolio"
     >
        <img src="~/assets/img/Coding_SVG.svg" alt slot="svg" style="height:80%"/>
      </feature-right>
      
      <feature-left
        headline="Digital Marketing & Social Media Management"
        content="My extensive experience in programming, finance, accounting, sales, trading, eCommerce and digital marketing allows me to be the best candidate to -"
        :list="smm"
        footer="Coupled with SEO, Automation tools and my programming skills."
        path="/smm"
        buttonName="Portfolio"
      >
        <img src="~/assets/img/Web_design_SVG.svg" alt slot="svg" style="height:80%" />
      </feature-left>

      <feature-right
        headline="Web Scraping"
        content="Through automated web scraping and data extraction convert websites to beautifully structured datasets. Suitable for Price Monitoring, Lead Generation, Marketing, Research etc."
        :list=web_scraping
        footer="Ease your life with quick access to datasets."
        path="/webscraping"
        buttonName="Portfolio"
     >
        <img src="~/assets/img/app_development_SVG.svg" alt slot="svg" style="height:80%"/>
      </feature-right>
    </div>
  </section>
</template>

<script>
import FeatureRight from '@/components/FeatureRight'
import FeatureLeft from '@/components/FeatureLeft'

export default {
  name: 'Features',
  data: function(){
    return{
      web_scraping: ['Directory Scraping', 'Price Monitoring', 'Lead Generation', 'Marketing', 'Research et'],
      smm: ['Maintain your online presence in your target communities', 'Curate information and threads for advertisement', 'Trigger natural growth', 'Sanitize your feed', 'Landing Pages'],
      automation_list: ['Custom Scripts', 'Interacting with Browsers', 'Microsoft Excel & Google Sheets', 'Microsoft Office Suite, PDF, OCR, Images', 'Interacting with Softwares, Desktop & Graphical User Interface (GUI)']
    }
  },
  components: {
    'feature-right': FeatureRight,
    'feature-left': FeatureLeft
  }
}
</script>
