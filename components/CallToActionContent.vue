<template>
  <section class="container mx-auto text-center py-6 mb-12">
    <h1
      class="w-full my-2 text-5xl font-bold leading-tight text-center text-white"
    >
      Glad to have you here
    </h1>
    <div class="w-full mb-4">
      <div
        class="h-1 mx-auto bg-white w-1/6 opacity-25 my-0 py-0 rounded-t"
      ></div>
    </div>

    <h3 class="my-4 text-3xl leading-tight">
      If you are interested, feel free to send me an email.
    </h3>
    <!-- <p>
      <button class="js-textareacopybtn" style="vertical-align:top;">
        Copy Textarea
      </button>
      <textarea class="js-copytextarea">Hello I'm some text</textarea>
    </p> -->
    <!-- <input type="text" v-model="message" /> -->
    <button
      class="mx-auto lg:mx-0 hover:underline bg-white text-gray-800 font-bold rounded-full my-6 py-4 px-8 shadow-lg"
      v-clipboard:copy="message"
      v-clipboard:success="onCopy"
      v-clipboard:error="onError"
    >
      <!-- Click To Copy My Email ! -->
      {{ button_text }}
    </button>
  </section>
</template>

<script>
import Vue from 'vue'
import VueClipboard from 'vue-clipboard2'

Vue.use(VueClipboard)

// $(document).ready(function() {
//   //call your script.js function from here
//   var copyTextareaBtn = document.querySelector('.js-textareacopybtn')

//   copyTextareaBtn.addEventListener('click', function(event) {
//     var copyTextarea = document.querySelector('.js-copytextarea')
//     copyTextarea.focus()
//     copyTextarea.select()

//     try {
//       var successful = document.execCommand('copy')
//       var msg = successful ? 'successful' : 'unsuccessful'
//       console.log('Copying text command was ' + msg)
//     } catch (err) {
//       console.log('Oops, unable to copy')
//     }
//   })
// })

export default {
  name: 'CallToActionContent',
  data: function() {
    return {
      message: 'anyfactor@gmail.com',
      button_text: 'Click to Get Email'
    }
  },
  methods: {
    onCopy: function(e) {
      alert(
        'Thanks for copying my Email\n\n' +
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
