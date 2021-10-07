<script>
  import { onMount } from 'svelte';

  onMount(() => {
    const btn = document.querySelector('button.mobile-menu-button');
    const menu = document.querySelector('.mobile-menu');

    btn.addEventListener('click', () => {
      menu.classList.toggle('hidden');
    });
  });
</script>

cs

<nav class="bg-white shadow-lg">
  <div class="max-w-6xl mx-auto px-4">
    <div class="flex justify-between">
      <div class="flex space-x-7">
        <!-- Website Logo -->
        <div>
          <a href="/" class="flex items-center py-4 px-2">
            <img src="logo.png" alt="Logo" class="h-8 w-8 mr-2" />
            <span class="font-semibold text-gray-500 text-lg">Navigation</span>
          </a>
        </div>
        <!-- Primary Navbar items -->
        <div class="hidden md:flex items-center space-x-1">
          <a
            href="/"
            class="py-4 px-2 text-green-500 border-b-4 border-green-500 font-semibold "
            >Home</a
          >
          <a
            href="services"
            class="py-4 px-2 text-gray-500 font-semibold hover:text-green-500 transition duration-300"
            >Services</a
          >
          <a
            href="about"
            class="py-4 px-2 text-gray-500 font-semibold hover:text-green-500 transition duration-300"
            >About</a
          >
          <a
            href="contact-us"
            class="py-4 px-2 text-gray-500 font-semibold hover:text-green-500 transition duration-300"
            >Contact Us</a
          >
        </div>
      </div>
    </div>
  </div>
</nav>
