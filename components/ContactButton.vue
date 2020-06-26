<template>
    <button
      class="mx-auto lg:mx-0 hover:underline bg-white text-gray-800 font-bold rounded-full my-6 py-4 px-8 shadow-lg"
      v-clipboard:copy="message"
      v-clipboard:success="onCopy"
      v-clipboard:error="onError"
    >
      <!-- Click To Copy My Email ! -->
      {{ button_text }}
    </button>
</template>
<script>
import VueClipboard from 'vue-clipboard2'
import Vue from 'vue'
Vue.use(VueClipboard)

export default {
  props: {
    message: {
      type: String,
      default: 'anyfactor@gmail.com',
      required: false
    },
    button_text: {
      type: String,
      default: 'Click to Get Email',
      required: false
    },
  },
  // data: function() {
  //   return {
  //     message: 'anyfactor@gmail.com',
  //     button_text: 'Click to Get Email'
  //   }
  // },
  methods: {
    onCopy: function(e) {
      alert(
        'Thanks for copying my contact info\n\n' +
          e.text +
          '\n\n Feel free to reach out to me anytime.'
      )
      this.button_text = this.message
    },
    onError: function(e) {
      alert('My Email is: anyfactor@gmail.com')
    }
  }
}
</script>