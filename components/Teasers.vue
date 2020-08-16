<template>
  <section class="bg-white border-b py-8">
    <div class="container mx-auto flex flex-wrap pt-4 pb-12">
      <h1
        class="w-full my-2 text-5xl font-bold leading-tight text-center text-gray-800"
      >
        Other Services
      </h1>
      <div class="w-full mb-4">
        <div
          class="h-1 mx-auto gradient w-64 opacity-25 my-0 py-0 rounded-t"
        ></div>
      </div>
      <!-- <teaser-column :rows="3" action="Portfolio" path="/webscraping">
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
      <teaser-column :rows="3" action="Portfolio" path="/automation">
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
      </teaser-column> -->
    </div>
    <div class="container mx-auto flex flex-wrap pt-4 pb-12">
      <teaser-column :rows="3" action="Portfolio" buttonBool path="/dataanalytics">
        <template v-slot:headline
          >Data Analytics & Visualization</template
        >
        <template v-slot:content
          >Convert your messy data and derive value-adding decision-making solutions. With Data cleanup, sanitization and structuring data-driven decision making can be done efficiently.<br/><br/>I can also help visualize your data and in static and dynamic form even in interactive web format media in SVG and Javascript.
        </template>
      </teaser-column>

    <teaser-column :rows="3" action="Details" buttonBool path="/webdev">
        <template v-slot:headline
          >Web<br/>Development</template
        >
        <template v-slot:content
          >
          I will help you create a beautiful, lightweight and user-focused website that is easy to operate and close as free to maintain.
        </template>
        <template v-slot:list>
          <li>Modifying Templates or Existing Projects</li>
          <li>Blog</li>
          <li>ECommerce</li>
          <li>Content Management System</li>
        </template>
        <template v-slot:footer
          >Currently looking for opportunities in a small team.
        </template>
      </teaser-column>


      <teaser-column :rows="3" action="Details">
        <template v-slot:headline
          >Python<br/>Programming</template
        >
        <template v-slot:content
          >I have been a professional python developer for years now. While some take python as a tool or merely a programming language, my use case of python derives from the passion I feel for it.<br/><br/>That is why I have explored and learned the extensive application of python. 

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
