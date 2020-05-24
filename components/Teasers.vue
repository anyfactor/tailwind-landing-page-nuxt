<template>
  <section class="bg-white border-b py-8">
    <div class="container mx-auto flex flex-wrap pt-4 pb-12">
      <h1
        class="w-full my-2 text-5xl font-bold leading-tight text-center text-gray-800"
      >
        Experience
      </h1>
      <div class="w-full mb-4">
        <div
          class="h-1 mx-auto gradient w-64 opacity-25 my-0 py-0 rounded-t"
        ></div>
      </div>
      <teaser-column :rows="3" action="Action">
        <template v-slot:headline
          >Web Scraping</template
        >
        <template v-slot:content
          >Through automated web scraping and data extraction convert websites
          to beautifully structured datasets. Suitable for Price Monitoring,
          Lead Generation, Marketing, Research etc.
        </template>
        <template v-slot:list>
          <li>Directory Scraping</li>
          <li>Price Monitoring</li>
          <li>Lead Generation</li>
          <li>Marketing</li>
          <li>Research etc.</li>
        </template>
        <template v-slot:footer
          >Ease your life with quick access to datasets.
        </template>
      </teaser-column>
      <teaser-column :rows="3" action="Action">
        <template v-slot:headline
          >Web Development</template
        >
        <template v-slot:content
          >I will help you create a beautiful, lightweight and user-focused
          website that is easy to operate and close as free to maintain.
        </template>
        <template v-slot:list>
          <li>Landing Pages</li>
          <li>Modifying Templates or Existing Projects</li>
          <li>Blog</li>
          <li>ECommerce</li>
          <li>Content Management System</li>
        </template>
        <template v-slot:footer
          >Whatever it is send me an email and we will make dreams into reality.
        </template>
      </teaser-column>
      <teaser-column :rows="3" action="Action">
        <template v-slot:headline
          >Automation</template
        >
        <template v-slot:content
          >I can create scripts to automate your boring repetitive tasks.
          Whatever you can think of
        </template>
        <template v-slot:list>
          <li>Custom Scripts</li>
          <li>Interacting with Browsers</li>
          <li>Microsoft Excel & Google Sheets</li>
          <li>Microsoft Office Suite, PDF, OCR, Images</li>
          <li>
            Interacting with Softwares, Desktop & Graphical User Interface (GUI)
          </li>
        </template>
        <template v-slot:footer
          >I will set up scripts using Remote Assistance and will provide
          detailed video instruction.
        </template>
      </teaser-column>
    </div>
    <div class="container mx-auto flex flex-wrap pt-4 pb-12">
      <teaser-column :rows="3" action="Action">
        <template v-slot:headline
          >Data Visualization</template
        >
        <template v-slot:content
          >Want to visualize your data for ease of understanding? With Excel and
          Python, I can help visualize your data and in static and dynamic form
          even in interactive web format media in SVG and Javascript.
        </template>
      </teaser-column>
      <teaser-column :rows="3" action="Action">
        <template v-slot:headline
          >Social Media Management</template
        >
        <template v-slot:content
          >My extensive experience in programming, finance, accounting, sales,
          eCommerce and digital marketing allows me to be the best candidate to
          -
        </template>
        <template v-slot:list>
          <li>Maintain your online presence in your target communities</li>
          <li>Curate information and threads for advertisement</li>
          <li>Trigger natural growth</li>
          <li>Sanitize your feed</li>
        </template>
        <template v-slot:footer
          >Coupled with SEO, Automation tools and my programming skills.
        </template>
      </teaser-column>
      <teaser-column :rows="3" action="Action">
        <template v-slot:headline
          >Data Analytics</template
        >
        <template v-slot:content
          >Convert your messy data and derive value-adding decision-making
          solutions. With my intermediate skills in MS Excel (Pivot Table,
          PowerQuery) and Python using Pandas, Numpy, SQL, Regex, CSV and
          service interaction data-driven decision making can be done
          efficiently.
        </template>
      </teaser-column>
    </div>
  </section>
</template>

<script>
import TeaserColumn from '@/components/TeaserColumn'

export default {
  name: 'Teasers',
  components: {
    'teaser-column': TeaserColumn
  }
}
</script>
