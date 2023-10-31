<!-- Navbar.svelte -->
  <script>
    let isMenuOpen = false;
    let isDropdownOpen = false;
  
    function toggleMenu() {
      isMenuOpen = !isMenuOpen;
    }
  
    function toggleDropdown() {
      isDropdownOpen = !isDropdownOpen;
    }


  </script>
  
  <nav class="bg-white p-4">
    <div class="container mx-auto px-4 py-2 flex justify-between items-center">
      <div class="text-black font-bold text-lg cursor-pointer">Your Logo</div>
      
      <div class="lg:hidden">
        <button class="text-black hover:text-yellow-500 duration-150 focus:outline-none" on:click={toggleMenu}>
            <svg xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><style>svg{fill:#000000}</style><path d="M0 96C0 78.3 14.3 64 32 64H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32C14.3 128 0 113.7 0 96zM0 256c0-17.7 14.3-32 32-32H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32c-17.7 0-32-14.3-32-32zM448 416c0 17.7-14.3 32-32 32H32c-17.7 0-32-14.3-32-32s14.3-32 32-32H416c17.7 0 32 14.3 32 32z"/></svg>
        </button>
      </div>
  
      <ul class="hidden lg:flex space-x-4">
        <li><a href="index" class="text-black hover:text-yellow-500 duration-150 text-xl px-2">Home</a></li>
        <li><a href="about" class="text-black hover:text-yellow-500 duration-150 text-xl px-2">About</a></li>
        <li><a href="mealkits" class="text-black hover:text-yellow-500 duration-150 text-xl px-2">Mealkits</a></li>
        <li on:click={toggleDropdown} class="cursor-pointer pt-1.5">
          <div> 
          <svg xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 512 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M233.4 406.6c12.5 12.5 32.8 12.5 45.3 0l192-192c12.5-12.5 12.5-32.8 0-45.3s-32.8-12.5-45.3 0L256 338.7 86.6 169.4c-12.5-12.5-32.8-12.5-45.3 0s-12.5 32.8 0 45.3l192 192z"/></svg> 
          {#if isDropdownOpen}
            <ul class="absolute bg-white mt-2 p-2 space-y-2 text-black">
              <li><a href="#" class="hover:text-gray-300">Option 1</a></li>
              <li><a href="#" class="hover:text-gray-300">Option 2</a></li>
            </ul>
          {/if}
          </div>
        </li>
        <li><a href="faq" class="text-black hover:text-yellow-500 duration-150 text-xl px-2">FAQ</a></li>
        <li><a href="contact" class="text-black hover:text-yellow-500 duration-150 text-xl px-2">Contact Us</a></li>
      </ul>
    </div>
  </nav>
  
  {#if isMenuOpen}
    <div class="lg:hidden">
      <ul class="bg-white ease-in py-4 duration-150">
        <li><a href="index" class="block text-black hover:bg-gray-200 duration-150 pl-4 py-2 text-xl w-full">Home</a></li>
        <li><a href="about" class="block text-black hover:bg-gray-200 duration-150 pl-4 py-2 text-xl">About</a></li>
        <li><a href="faq" class="block text-black hover:bg-gray-200 duration-150 pl-4 py-2 text-xl">FAQ</a></li>
        <li><a href="contact" class="block text-black hover:bg-gray-200 duration-150 pl-4 py-2 text-xl">Contact Us</a></li>
      </ul>
    </div>
  {/if}