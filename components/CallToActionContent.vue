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
    <p>
      <button class="js-textareacopybtn" style="vertical-align:top;">
        Copy Textarea
      </button>
      <textarea class="js-copytextarea">Hello I'm some text</textarea>
    </p>

    <button
      class="mx-auto lg:mx-0 hover:underline bg-white text-gray-800 font-bold rounded-full my-6 py-4 px-8 shadow-lg"
      @click="doCopy"
    >
      <!-- Click To Copy My Email ! -->
      anyfactor@gmail.com
    </button>
  </section>
</template>

<script>
$(document).ready(function() {
  //call your script.js function from here
  var copyTextareaBtn = document.querySelector('.js-textareacopybtn')

  copyTextareaBtn.addEventListener('click', function(event) {
    var copyTextarea = document.querySelector('.js-copytextarea')
    copyTextarea.focus()
    copyTextarea.select()

    try {
      var successful = document.execCommand('copy')
      var msg = successful ? 'successful' : 'unsuccessful'
      console.log('Copying text command was ' + msg)
    } catch (err) {
      console.log('Oops, unable to copy')
    }
  })
})

export default {
  name: 'CallToActionContent'
}
</script>
