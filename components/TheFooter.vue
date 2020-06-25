<template>
  <footer class="bg-white">
    <div class="container mx-auto px-8">
      <div class="w-full flex flex-col md:flex-row py-6">
        <div class="flex-1 mb-6">
          <logo />
        </div>
        <div class="flex-1">
          <p class="uppercase text-gray-500 md:mb-6">Links</p>
          <ul class="list-reset mb-6">
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="#"
                class="no-underline hover:underline text-gray-800 hover:text-orange-500"
                >FAQ</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="#"
                class="no-underline hover:underline text-gray-800 hover:text-orange-500"
                >Help</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="#"
                class="no-underline hover:underline text-gray-800 hover:text-orange-500"
                >Terms</a
              >
            </li>
          </ul>
        </div>
        <div class="flex-1">
          <p class="uppercase text-gray-500 md:mb-6">Legal</p>
          <ul class="list-reset mb-6">
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="#"
                class="no-underline hover:underline text-gray-800 hover:text-orange-500"
                >Terms</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="#"
                class="no-underline hover:underline text-gray-800 hover:text-orange-500"
                >Privacy</a
              >
            </li>
          </ul>
        </div>
        <div class="flex-1">
          <p class="uppercase text-gray-500 md:mb-6">Social</p>
          <ul class="list-reset mb-6">
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="https://reddit.com/u/anyfactor" target="_blank" 
                class="no-underline hover:underline text-gray-800 hover:text-orange-500"
                >Reddit</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="https://twitter.com/anyfactor" target="_blank" 
                class="no-underline hover:underline text-gray-800 hover:text-orange-500"
                >Twitter</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="https://www.youtube.com/channel/UCYtdDWgkfAnNSxL37s6SWLQ" target="_blank" 
                class="no-underline hover:underline text-gray-800 hover:text-orange-500"
                >YouTube</a
              >
            </li>
          </ul>
        </div>
        <div class="flex-1">
          <p class="uppercase text-gray-500 md:mb-6">Developer Links</p>
          <ul class="list-reset mb-6">
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="https://github.com/anyfactor/" target="_blank" 
                class="no-underline hover:underline text-gray-800 hover:text-orange-500"
                >Github</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="https://www.codewars.com/users/anyfactor" target="_blank" 
                class="no-underline hover:underline text-gray-800 hover:text-orange-500"
                >CodeWars</a
              >
            </li>
            <li class="mt-2 inline-block mr-2 md:block md:mr-0">
              <a
                href="https://medium.com/@anyfactor/" target="_blank" 
                class="no-underline hover:underline text-gray-800 hover:text-orange-500"
                >Medium</a
              >
            </li>
          </ul>
        </div>
      </div>
    </div>

    <a href="https://www.freepik.com/free-photos-vectors/background"
      >Background vector created by freepik - www.freepik.com</a
    >
  </footer>
</template>

<script>
import Logo from '@/components/Logo'

export default {
  name: 'TheFooter',
  components: {
    logo: Logo
  }
}
</script>
