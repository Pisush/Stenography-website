<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup


const toggleMobileMenu = (evt: Event) => {
      const navMenu = document.querySelector('#nav-menu');
      navMenu?.classList.toggle('hidden');
}
</script>

<template>
  <div>
    <!-- nav -->
    <nav>
      <div class="container mx-auto px-6 py-2 flex justify-between items-center">
        <a class="font-bold text-2xl lg:text-4xl" href="#">Stenography</a>
        <!-- <div class="block lg:hidden">
          <button
            id="nav-toggle"
            @click="toggleMobileMenu"
            class="flex items-center px-3 py-2 border rounded text-gray-500 border-gray-600 hover:text-gray-800 hover:border-teal-500 appearance-none focus:outline-none"
          >
            <svg
              class="fill-current h-3 w-3"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg"
            >
              <title>Menu</title>
              <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
            </svg>
          </button>
        </div>
        <div class="hidden lg:block">
          <ul class="inline-flex">
            <li>
              <a class="px-4 font-bold" href="/">Home</a>
            </li>
            <li>
              <a class="px-4 hover:text-gray-800" href="#">About</a>
            </li>
            <li>
              <a class="px-4 hover:text-gray-800" href="#">Contact</a>
            </li>
          </ul>
        </div> -->
      </div>
    </nav>
    <!-- <div class="hidden" id="nav-menu">
      <ul class>
        <li class="active">
          <a
            href="index.html"
            class="block text-sm px-2 py-4 text-white bg-green-500 font-semibold"
          >Home</a>
        </li>
        <li>
          <a
            href="#about"
            class="block text-sm px-2 py-4 hover:bg-green-500 transition duration-300"
          >About</a>
        </li>
        <li>
          <a
            href="#contact"
            class="block text-sm px-2 py-4 hover:bg-green-500 transition duration-300"
          >Contact Us</a>
        </li>
      </ul>
    </div> -->

    <!-- hero -->
    <div class="py-20" style="background: linear-gradient(90deg, #BA5A31 0%, #FAF0CA 100%)">
      <div class="container mx-auto px-6">
        <h2
          class="text-4xl font-bold mb-2 text-white"
        >Using AI to make code more accessible to everyone</h2>
        <h3 class="text-2xl mb-8 text-gray-200">Powered by GPT-3</h3>
      </div>
    </div>
  </div>
  <!-- features -->
  <section class="container mx-auto px-6 p-10">
    <h2 class="text-4xl font-bold text-center text-gray-800 mb-8">Features</h2>

    <div class="flex items-center flex-wrap mb-20">
      <div class="w-full md:w-1/2">
        <h4 class="text-3xl text-gray-800 font-bold mb-3">A Powerful API</h4>
        <p
          class="text-xl mb-8"
        >Prioritizes simplicity: pass in some code, recieve an explanation.</p>
      </div>
      <div class="w-full md:w-1/2 pl-2">
        <img src="./assets/steno-api-landing-page.png" alt="api" />
      </div>
    </div>

    <div class="flex items-center flex-wrap mb-20">
      <div class="w-full md:w-1/2">
        <img src="./assets/vsc.gif" alt="vsc" />
      </div>
      <div class="w-full md:w-1/2 pl-8">
        <h4 class="text-3xl text-gray-800 font-bold mb-3">Extensions: VSC</h4>
        <p class="text-xl mb-8">Auto document your code. Leverage creative commenting.</p>
      </div>
    </div>

    <div class="flex items-center flex-wrap mb-20">
      <div class="w-full md:w-1/2">
        <h4 class="text-3xl text-gray-800 font-bold mb-3">Extensions: Chrome</h4>
        <p
          class="text-xl mb-8"
        >Discover what that code means in GitHub or StackOverflow or on someone's blog.</p>
      </div>
      <div class="w-full md:w-1/2 pl-2">
        <img src="./assets/chrome.gif" alt="chrome" />
      </div>
    </div>

    <div class="flex items-center flex-wrap mb-20">
      <div class="w-full md:w-1/2">
        <img src="./assets/slack.gif" alt="slack" />
      </div>
      <div class="w-full md:w-1/2 pl-8">
        <h4 class="text-3xl text-gray-800 font-bold mb-3">Extensions: Slack/Discord</h4>
        <p
          class="text-xl mb-8"
        >Don't stop a conversation between team members to read code.</p>
      </div>
    </div>
  </section>
  <!-- testimonials -->
  <!-- <section class="bg-gray-100">
    <div class="container mx-auto px-6 py-20">
      <h2 class="text-4xl font-bold text-center text-gray-800 mb-8">Testimonials</h2>
      <div class="flex flex-wrap">
        <div class="w-full md:w-1/3 px-2 mb-4">
          <div class="bg-white rounded shadow py-2">
            <p
              class="text-gray-800 text-base px-6 mb-5"
            >Monitoring and tracking my health vitals anywhere I go and on any platform I use has never been easier.</p>
            <p class="text-gray-500 text-xs md:text-sm px-6">John Doe</p>
          </div>
        </div>
        <div class="w-full md:w-1/3 px-2 mb-4">
          <div class="bg-white rounded shadow py-2">
            <p
              class="text-gray-800 text-base px-6 mb-5"
            >As an Athlete, this is the perfect product for me. I wear my Smart Health Monitoring Wristwatch everywhere I go, even in the bathroom since it's waterproof.</p>
            <p class="text-gray-500 text-xs md:text-sm px-6">Jane Doe</p>
          </div>
        </div>
        <div class="w-full md:w-1/3 px-2 mb-4">
          <div class="bg-white rounded shadow py-2">
            <p
              class="text-gray-800 text-base px-6 mb-5"
            >I don't regret buying this wearble gadget. One of the best gadgets I own!.</p>
            <p class="text-gray-500 text-xs md:text-sm px-6">James Doe</p>
          </div>
        </div>
      </div>
    </div>
  </section> -->
  <!-- cta -->
  <section style="background-color: #FAF0CA">
    <div class="container mx-auto px-6 text-center py-20">
      <h2 class="mb-6 text-4xl font-bold text-center text-black">Join the Discord</h2>
      <h3 class="my-4 text-2xl text-black">Want live updates about the product? Want to try using Stenography today? Join the Discord!</h3>
      <!-- <button
        class="bg-white font-bold rounded-full mt-6 py-4 px-8 shadow-lg uppercase tracking-wider"
      >Pre Order</button> -->
      <a target='_blank' href='https://discord.com/invite/FgMxkfVwxk' style='font-size:24px; background-color: #738adb; color: white; border-radius: 6px; border-width: 0px; padding: 12px;text-decoration: none;color: white;'>Join the Discord <i class='fab fa-discord'></i></a>
    </div>
  </section>
  <!-- footer -->
  <footer class="bg-gray-100">
    <div class="container mx-auto px-6 pt-10 pb-6">
      <div class="flex flex-wrap">
        <!-- <div class="w-full md:w-1/4 text-center md:text-left">
          <h5 class="uppercase mb-6 font-bold">Links</h5>
          <ul class="mb-4">
            <li class="mt-2">
              <a href="#" class="hover:underline text-gray-600 hover:text-orange-500">FAQ</a>
            </li>
            <li class="mt-2">
              <a href="#" class="hover:underline text-gray-600 hover:text-orange-500">Help</a>
            </li>
            <li class="mt-2">
              <a href="#" class="hover:underline text-gray-600 hover:text-orange-500">Support</a>
            </li>
          </ul>
        </div> -->
        <div class="w-full md:w-1/4 text-center md:text-left">
          <h5 class="uppercase mb-6 font-bold">Legal</h5>
          <ul class="mb-4">
            <li class="mt-2">
              <a href="#" class="hover:underline text-gray-600 hover:text-orange-500">Terms</a>
            </li>
            <li class="mt-2">
              <a href="#" class="hover:underline text-gray-600 hover:text-orange-500">Privacy</a>
            </li>
          </ul>
        </div>
        <div class="w-full md:w-1/4 text-center md:text-left">
          <h5 class="uppercase mb-6 font-bold">Social</h5>
          <ul class="mb-4">
            <li class="mt-2">
              <a href="#" class="hover:underline text-gray-600 hover:text-orange-500">Twitter</a>
            </li>
          </ul>
        </div>
        <div class="w-full md:w-1/4 text-center md:text-left">
          <h5 class="uppercase mb-6 font-bold">Company</h5>
          <ul class="mb-4">
            <li class="mt-2">
              <a href="#" class="hover:underline text-gray-600 hover:text-orange-500">Official Blog</a>
            </li>
            <!-- <li class="mt-2">
              <a href="#" class="hover:underline text-gray-600 hover:text-orange-500">About Us</a>
            </li>
            <li class="mt-2">
              <a href="#" class="hover:underline text-gray-600 hover:text-orange-500">Contact</a>
            </li> -->
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

