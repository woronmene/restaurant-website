<script>
  let isMobileMenuOpen = false;

  function toggleMobileMenu() {
    isMobileMenuOpen = !isMobileMenuOpen;
  }
</script>

<nav class="fixed w-full">
    <div class="w-full relative  bg-white">
        <div class="w-full px-5 md:px-10 flex items-center gap-[50px] lg:gap-[100px] xl:gap-[200px] py-1 ">
            <div class="w-[140px] flex-0 cursor-pointer">
                <img class="w-full" src="/logo.png" alt="">
            </div>

            <div class="flex-1 hidden lg:block py-2 ">

                    <div class="flex lg:w-2/3 xl:w-1/2 justify-between text-xs tracking-3">
                        <li class="duration-200 hover:text-[#FF6244]">
                            <a href="#hero">
                                hOME
                            </a>
                        </li>
                        <li class="duration-200 hover:text-[#FF6244]">
                            <a href="#menu">
                                oUR MENU
                            </a>
                        </li>
                        <li class="duration-200 hover:text-[#FF6244]">
                            <a href="#cta">
                            gET IN TOUCH
                            </a>
                        </li>
                    
                    </div>
            </div>

               <button class="lg:hidden absolute top-[50%] -translate-y-[50%] right-[10px] cursor-pointer" on:click={toggleMobileMenu}>
                 <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            d="M4 6h16M4 12h16m-7 6h7"></path>
        </svg>
        </button>
        

        </div>

     






<div class={`lg:hidden ${isMobileMenuOpen ? 'right-0' : 'right-[-100%]'} fixed top-0  h-full w-full md:w-1/2 bg-white transition-all ease-in-out duration-300 z-50`}>

    <div class="p-4 mt-20 ">
      <a href="#hero" class="block py-2 hover:text-[#FF6244] cursor-pointer" on:click={toggleMobileMenu}>hOME</a>
      <a href="#menu" class="block py-2 hover:text-[#FF6244] cursor-pointer" on:click={toggleMobileMenu}> oUR MENU</a>
      <a href="#cta" class="block py-2 hover:text-[#FF6244] cursor-pointer" on:click={toggleMobileMenu}> gET IN TOUCH</a>
    </div>

    <button class="absolute top-3 right-3 cursor-pointer" on:click={toggleMobileMenu}>
        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"
  xmlns="http://www.w3.org/2000/svg">
  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
    d="M6 18L18 6M6 6l12 12"></path>
</svg>
    </button>
  </div>
    </div>
    <div class="w-full py-4 bg-[#FF6244]">

    </div>
</nav>