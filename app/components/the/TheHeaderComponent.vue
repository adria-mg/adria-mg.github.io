<script setup>
  /*var toggleOpen = document.getElementById('toggleOpen');
  var toggleClose = document.getElementById('toggleClose');
  var collapseMenu = document.getElementById('collapseMenu');

  function handleClick() {
    if (collapseMenu.style.display === 'block') {
      collapseMenu.style.display = 'none';
    } else {
      collapseMenu.style.display = 'block';
    }
  }

  window.onload=function(){
  toggleOpen.addEventListener('click', handleClick);
  toggleClose.addEventListener('click', handleClick);
}
  */
</script>

<template>
  
    <header class="shadow-md tracking-wide relative z-50">
      <!--
      <section class="py-2 bg-lightblue text-blue text-right px-10">
        <p class="text-sm">
          <span class="mx-1 font-semibold">
            Contacto:
          </span>
          info@aecie.org
        </p>
      </section>
    -->

      <div class="flex flex-wrap items-center justify-between gap-4 px-10 py-3 bg-blue min-h-[65px]">
        <a href="javascript:void(0)">
          <!--<NuxtImg src="/LogoEuropeCat_2025.png" alt="logo" class="w-20"/>-->
          <!--<img src="./assets/images/LogoEuropeCat_2025.png" alt="logo" class="w-20" />-->
        </a>

        <div id="collapseMenu"
          class="max-lg:hidden lg:!block max-lg:before:fixed max-lg:before:bg-black max-lg:before:opacity-50 max-lg:before:inset-0 max-lg:before:z-50">
          <button id="toggleClose" class="lg:hidden fixed top-2 right-4 z-[100] rounded-full bg-white w-9 h-9 flex items-center justify-center border border-gray-200 cursor-pointer">
            <svg xmlns="http://www.w3.org/2000/svg" class="w-3.5 h-3.5 fill-white" viewBox="0 0 320.591 320.591">
              <path
                d="M30.391 318.583a30.37 30.37 0 0 1-21.56-7.288c-11.774-11.844-11.774-30.973 0-42.817L266.643 10.665c12.246-11.459 31.462-10.822 42.921 1.424 10.362 11.074 10.966 28.095 1.414 39.875L51.647 311.295a30.366 30.366 0 0 1-21.256 7.288z"
                data-original="#000000"></path>
              <path
                d="M287.9 318.583a30.37 30.37 0 0 1-21.257-8.806L8.83 51.963C-2.078 39.225-.595 20.055 12.143 9.146c11.369-9.736 28.136-9.736 39.504 0l259.331 257.813c12.243 11.462 12.876 30.679 1.414 42.922-.456.487-.927.958-1.414 1.414a30.368 30.368 0 0 1-23.078 7.288z"
                data-original="#000000"></path>
            </svg>
          </button>

          <ul
            class="lg:flex lg:gap-x-5 max-lg:space-y-3 max-lg:fixed max-lg:bg-white max-lg:w-1/2 max-lg:min-w-[300px] max-lg:top-0 max-lg:left-0 max-lg:p-6 max-lg:h-full max-lg:shadow-md max-lg:overflow-auto z-50">
            <li class="mb-6 hidden max-lg:block">
              <a href="javascript:void(0)"><img src="/LogoEuropeCat_2025.png" alt="logo" class="w-36" />
              </a>
            </li>
            <li class="max-lg:border-b max-lg:border-gray-300 max-lg:py-3 px-3">
              <a href='javascript:void(0)'
                class="hover:text-red text-white font-medium text-[15px]"> 
                Inicio
              </a>
            </li>
            <li class="max-lg:border-b max-lg:border-gray-300 max-lg:py-3 px-3"><a href='javascript:void(0)'
              class="hover:text-red text-white block font-medium text-[15px]">Clase</a>
            </li>
            <li class="max-lg:border-b max-lg:border-gray-300 max-lg:py-3 px-3"><a href='javascript:void(0)'
              class="hover:text-red text-white block font-medium text-[15px]">Notícias</a>
            </li>
            <li class="max-lg:border-b max-lg:border-gray-300 max-lg:py-3 px-3"><a href='javascript:void(0)'
              class="hover:text-red text-white block font-medium text-[15px]">Calendario</a>
            </li>
            <li class="max-lg:border-b max-lg:border-gray-300 max-lg:py-3 px-3"><a href='javascript:void(0)'
              class="hover:text-red text-white block font-medium text-[15px]">
              Ránquing</a>
            </li>
            <li class="max-lg:border-b max-lg:border-gray-300 max-lg:py-3 px-3"><a href='javascript:void(0)'
              class="hover:text-red text-white block font-medium text-[15px]">Compra-Venta</a>
            </li>
     
            <li class="max-lg:border-b max-lg:border-gray-300 max-lg:py-3 px-3"><a href='javascript:void(0)'
              class="hover:text-red text-white block font-medium text-[15px]">Contacto</a>
            </li>
          </ul>
        </div>

        <div class="flex max-lg:ml-auto">
          <button id="toggleOpen" class="lg:hidden cursor-pointer">
            <svg class="w-7 h-7" fill="#000" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd"
                d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
                clip-rule="evenodd"></path>
            </svg>
          </button>
          <span class="mx-3 flex items-center">
          <button type="button" class="flex items-center text-white bg-red hover:bg-lightblue hover:text-blue focus:outline-none font-medium rounded-full text-sm px-5 py-2.5 text-center me-2 mb-2">
            <span class="solar--user-bold mr-2"></span>
            Acceso regatistas
          </button>
        </span>
        </div>
      </div>
    </header>
</template>

<style>
  .solar--user-bold {
    display: inline-block;
    width: 18px;
    height: 18px;
    background-repeat: no-repeat;
    background-size: 100% 100%;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Ccircle cx='12' cy='6' r='4' fill='%23fff'/%3E%3Cpath fill='%23fff' d='M20 17.5c0 2.485 0 4.5-8 4.5s-8-2.015-8-4.5S7.582 13 12 13s8 2.015 8 4.5'/%3E%3C/svg%3E");
  }

  .material-symbols--home-rounded {
  display: inline-block;
  width: 24px;
  height: 24px;
  --svg: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath fill='%23000' d='M4 19v-9q0-.475.213-.9t.587-.7l6-4.5q.525-.4 1.2-.4t1.2.4l6 4.5q.375.275.588.7T20 10v9q0 .825-.588 1.413T18 21h-3q-.425 0-.712-.288T14 20v-5q0-.425-.288-.712T13 14h-2q-.425 0-.712.288T10 15v5q0 .425-.288.713T9 21H6q-.825 0-1.412-.587T4 19'/%3E%3C/svg%3E");
  background-color: currentColor;
  -webkit-mask-image: var(--svg);
  mask-image: var(--svg);
  -webkit-mask-repeat: no-repeat;
  mask-repeat: no-repeat;
  -webkit-mask-size: 100% 100%;
  mask-size: 100% 100%;
}
</style>