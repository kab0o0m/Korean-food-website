<!-- Navbar.svelte -->
<script>
  import ProductCounter from "$lib/product_counter.svelte";

  let isMenuOpen = false;
  let isDropdownOpen = false;
  let isCartOpen = false;
  
  const dropdownFocus = () => { isDropdownOpen = true; }
  const dropdownBlur = () => { isDropdownOpen = false; }
  
  const cartFocus = () => { isCartOpen = true; }
  const cartBlur= () => { isCartOpen = false; }
  
  function toggleDropdown() {
    isDropdownOpen = !isDropdownOpen;
  }
  function toggleCart() {
    isCartOpen = !isCartOpen;
  }
  function toggleMenu() {
    isMenuOpen = !isMenuOpen;
  }
</script>

<nav class="bg-white z-50  px-3 sm:px-3 md:px-3 lg:p-1 xl:p-1 2xl:p-1 fixed w-screen shadow-xl select-none">
  <div class="container mx-auto px-4 py-2 flex justify-between items-center">
    <a class="cursor-pointer text-xl" href="home">
      <img class="h-16 w-auto" src="assets/logo.jpg" alt=""/>
    </a>
    <ul class="hidden lg:flex space-x-10">
      <li class="flex content-center justify-center"><a href="home" class="text-black hover:text-yellow-500 duration-150 text-xl px-2 pt-1">Home</a></li>
      <li class="flex content-center justify-center"><a href="about" class="text-black hover:text-yellow-500 duration-150 text-xl px-2 pt-1">About</a></li>
      <li>
        <div class="flex relative pt-1">
          <a href="mealkits" class="text-black hover:text-yellow-500 duration-150 text-xl px-2">Mealkits</a>
          <!-- svelte-ignore a11y-click-events-have-key-events -->
          <!-- svelte-ignore a11y-no-static-element-interactions -->
          <div class="cursor-pointer pt-1.5 relative">
            <button class="hover:scale-125 pl-1 pb-2 duration-150" on:click={toggleDropdown} >
              { #if isDropdownOpen }
                <svg xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 512 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M233.4 105.4c12.5-12.5 32.8-12.5 45.3 0l192 192c12.5 12.5 12.5 32.8 0 45.3s-32.8 12.5-45.3 0L256 173.3 86.6 342.6c-12.5 12.5-32.8 12.5-45.3 0s-12.5-32.8 0-45.3l192-192z"/></svg>
              { :else }
                <svg xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 512 512">
                <path d="M233.4 406.6c12.5 12.5 32.8 12.5 45.3 0l192-192c12.5-12.5 12.5-32.8 0-45.3s-32.8-12.5-45.3 0L256 338.7 86.6 169.4c-12.5-12.5-32.8-12.5-45.3 0s-12.5 32.8 0 45.3l192 192z"/>
                </svg>
              {/if}
            </button>
            </div>
            {#if isDropdownOpen}
              <ul class="py-4 bg-white text-black rounded-lg text-center absolute -top-6 mt-16 -left-14 w-max shadow-xl">
                <a href="beef"><li class="px-4 py-1 text-xl hover:bg-gray-200">Beef Bulgogi</li></a>
                <a href="chicken"><li class="px-4 py-1 text-xl hover:bg-gray-200">Spicy Chicken Bulgogi</li></a>
                <a href="pork"><li class="px-4 py-1 text-xl hover:bg-gray-200">Spicy Pork Bulgogi</li></a>
                <a href="armystew"><li class="px-4 py-1 text-xl hover:bg-gray-200">Army Stew</li></a>
              </ul>
            {/if}
          </div>
        </li>
        <li class="flex content-center justify-center"><a href="faq" class="text-black hover:text-yellow-500 duration-150 text-xl px-2 pt-1">FAQ</a></li>
        <li class="flex content-center justify-center"><a href="contact" class="text-black hover:text-yellow-500 duration-150 text-xl px-2 pt-1">Contact Us</a></li>
        <li class="pt-1">
          <div class="relative">
            <!-- svelte-ignore a11y-no-static-element-interactions -->
            <!-- svelte-ignore a11y-click-events-have-key-events -->
            <button class="bg-primary-500  px-6 py-2 rounded-xl cursor-pointer relative hover:bg-primary-400" on:click={toggleCart}>
              {#if isCartOpen}
                <svg xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 512 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M233.4 105.4c12.5-12.5 32.8-12.5 45.3 0l192 192c12.5 12.5 12.5 32.8 0 45.3s-32.8 12.5-45.3 0L256 173.3 86.6 342.6c-12.5 12.5-32.8 12.5-45.3 0s-12.5-32.8 0-45.3l192-192z"/></svg>
              { :else }
                <svg xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 576 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M528.12 301.319l47.273-208C578.806 78.301 567.391 64 551.99 64H159.208l-9.166-44.81C147.758 8.021 137.93 0 126.529 0H24C10.745 0 0 10.745 0 24v16c0 13.255 10.745 24 24 24h69.883l70.248 343.435C147.325 417.1 136 435.222 136 456c0 30.928 25.072 56 56 56s56-25.072 56-56c0-15.674-6.447-29.835-16.824-40h209.647C430.447 426.165 424 440.326 424 456c0 30.928 25.072 56 56 56s56-25.072 56-56c0-22.172-12.888-41.332-31.579-50.405l5.517-24.276c3.413-15.018-8.002-29.319-23.403-29.319H218.117l-6.545-32h293.145c11.206 0 20.92-7.754 23.403-18.681z"/></svg>
                <div class="absolute inline-flex items-center justify-center w-6 h-6 text-sm pb-0.5 font-bold text-white bg-red-500 border-2 border-white rounded-full -top-2 -right-2 dark:border-gray-900">4</div>
              {/if}
            </button>
            {#if isCartOpen}
            <div class="px-2 py-3 mt-4 bg-white text-black rounded-lg text-center right-0 absolute w-max shadow-xl" on:blur={cartBlur}>
              <ul>
                <li class="h-24 w-full flex">
                  <div class="h-full w-24 pt-2 mr-2"><img src="./assets/beef_bulgogi_img.png" alt="" /></div>
                  <div class="p-2 text-left">
                    <p>Beef Bulgogi</p>
                    <p class="">$8.00</p>
                    <ProductCounter />
                  </div>
                </li>
                <hr class="py-1">
                <li class="h-24 w-full flex">
                  <div class="pt-2 mr-2 h-full w-24"><img src="./assets/spicy_chicken_bulgogi_img.png" alt="" /></div>
                  <div class="p-2 text-left">
                    <p>Spicy Chicken Bulgogi</p>
                    <p>$8.00</p>
                    <ProductCounter />
                  </div>
                </li>
                <hr class="py-1">
                <li class="h-24 w-full flex">
                  <div class="pt-2 mr-2 h-full w-24"><img src="./assets/spicy_pork_bulgogi_img.png" alt="" /></div>
                  <div class="p-2 text-left">
                    <p>Spicy Pork Bulgogi</p>
                    <p>$8.00</p>
                    <ProductCounter />
                  </div>
                </li>
                <hr class="py-1">
                <li class="h-24 w-full flex">
                  <div class="pt-2 mr-2 h-full w-24"><img src="./assets/army_stew_img.png" alt="" /></div>
                  <div class="p-2 text-left">
                    <p>Army Stew</p>
                    <p>$8.00</p>
                    <ProductCounter />
                  </div>
                </li>
              </ul>
              <div class="w-max flex justify-between">
                <p class="pt-2.5 font-bold text-lg">Subtotal: $32.00</p>
                <div class="w-24"><!-- spacer --></div>
                <a class="mt-2 py-1 px-2 flex items-center font-bold bg-primary-500 rounded-xl" href="checkout">Check Out &nbsp;<svg class="" xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M438.6 278.6c12.5-12.5 12.5-32.8 0-45.3l-160-160c-12.5-12.5-32.8-12.5-45.3 0s-12.5 32.8 0 45.3L338.8 224 32 224c-17.7 0-32 14.3-32 32s14.3 32 32 32l306.7 0L233.4 393.4c-12.5 12.5-12.5 32.8 0 45.3s32.8 12.5 45.3 0l160-160z"/></svg> </a>
              </div>
            </div>
            {/if}
          </div>
        </li>

      </ul>
      <div class="lg:hidden">
        <button class="m-2" on:click={toggleMenu}>
          { #if isMenuOpen }
          <svg xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 512 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M233.4 105.4c12.5-12.5 32.8-12.5 45.3 0l192 192c12.5 12.5 12.5 32.8 0 45.3s-32.8 12.5-45.3 0L256 173.3 86.6 342.6c-12.5 12.5-32.8 12.5-45.3 0s-12.5-32.8 0-45.3l192-192z"/></svg>
          { :else }
          <svg class="h-5 w-5" xmlns="http://www.w3.org/2000/svg" height="1em" viewBox="0 0 448 512">
            <path d="M0 96C0 78.3 14.3 64 32 64H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32C14.3 128 0 113.7 0 96zM0 256c0-17.7 14.3-32 32-32H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32c-17.7 0-32-14.3-32-32zM448 416c0 17.7-14.3 32-32 32H32c-17.7 0-32-14.3-32-32s14.3-32 32-32H416c17.7 0 32 14.3 32 32z"/>
          </svg>
          { /if }
        </button>
      </div>
    </div>
  </nav>
  
  {#if isMenuOpen}
  <div class="lg:hidden absolute top-20 z-50 shadown-xl w-screen border-b-4 border-gray-300">
    <ul class="bg-white z-50 py-4">
      <li class="py-1"><a href="home" class="block text-black hover:bg-gray-200 duration-150 pl-4 py-2 text-xl w-full">Home</a></li>
      <li class="py-1"><a href="about" class="block text-black hover:bg-gray-200 duration-150 pl-4 py-2 text-xl">About</a></li>
      <li class="py-1"><a href="faq" class="block text-black hover:bg-gray-200 duration-150 pl-4 py-2 text-xl">FAQ</a></li>
      <li class="py-1"><a href="contact" class="block text-black hover:bg-gray-200 duration-150 pl-4 py-2 text-xl">Contact Us</a></li>
      <li class="py-1"><a href="checkout" class="block text-black hover:bg-gray-200 duration-150 pl-4 py-2 text-xl">
        <div class="relative w-min">
          <p class="w-max">Check Out</p>
          <div class="absolute inline-flex items-center justify-center w-6 h-6 text-sm pb-0.5 font-bold text-white bg-red-500 border-2 border-white rounded-full -top-2 -right-6 dark:border-gray-900">4</div>
        </div>
      </a></li>
    </ul>
  </div>
  {/if}