<template>
  <section class="bg-white border-b py-8">
    <div class="container mx-auto flex flex-wrap pb-12">
      <h1
        class="w-full my-2 text-5xl font-bold leading-tight text-center text-gray-800"
      >
        Testimonials
      </h1>
      <div class="w-full mb-4">
        <div
          class="h-1 mx-auto gradient w-64 opacity-25 my-0 py-0 rounded-t"
        ></div>
      </div>
    </div>
    <div class="container mx-auto flex flex-wrap pt-4 pb-12">
      <div v-for="statement in testimonials" :key="statement.title">
        <teaser-column :rows="1" img_path="~/assets/img/programming.png">
        <template v-slot:headline
          >{{ statement.title }}</template
        >
        <template v-slot:content
          >{{ statement.statement }}</template>
      </teaser-column>
      </div>
    </div>
  </section>
</template>

<script>
import TeaserColumn from '@/components/TeaserColumn'

export default {
  components: {
    'teaser-column': TeaserColumn
  },
  data: function (){
    return {
      testimonials: [{'title': 'anyfactor diverse talents and eager to learn', 'statement': "I've had the pleasure of working with u/anyfactor on a number of different projects. He has created technical content, edited videos, managed social media accounts, and done VueJs development work.\n\nWhat impresses me most about u/anyfactor is his desire to learn and provide results for the client. He is a good communicator and cares about the projects he works on. He is open to feedback and is an all-round good person to work with."}, {'title': 'anyfactor helped me automate tasks using python', 'statement': 'Anyfactor helped me write and set up scripts for some ecommerce business. He then walked me through setting up the scripts and maintain regular correspondence to make sure the scripts work. Excellent pride of workmanship, he made sure everything worked on my end and helped me work through a few issues in my environment.\n\n10/10 would (and most likely will) work with him again. Highly recommended.'}, {'title': 'anyfactor Vue.JS developer', 'statement': 'I worked with AnyFactor on a series of tasks for a website. I found him responsive, communicative and overall good to work with.\n\nHe delivered before deadline, had a detailed account of his work, and achieved the desired outcomes.'}, {'title': 'anyfactor is doing a great job', 'statement': 'Very proactive and enthusiast in every way possible conducting social media accounts. You will find him constantly asking questions on how he can improve. He has been able to pick up the nuances of the business quickly, participates in the appropriate communities, and is very professional.\n\nHighly recommend him for any social media or dev needs. He is friendly and very easy to communicate with. It has been a pleasure working with him.'}, {'title': 'anyfactor is an awesome python developer', 'statement': 'Hired u/anyfactor for a fairly complicated python project. He was extremely quick to solve the problem. He kept me updated with the process and helped me walk through subsequent problems. He is a nice guy, easy to communicate with and he provided assurance for further assistance. 10/10. Highly recommended.'}]
    }
  }
}
</script>