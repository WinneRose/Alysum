<template>
  <!-- Section 1 -->
  <section class="w-full px-3 antialiased bg-gray-900 lg:px-6">
    <div class="mx-auto max-w-7xl">
      <nav
        class="flex items-center w-full h-24 select-none"
        x-data="{ showMenu: false }"
      >
        <div
          class="relative flex flex-wrap items-center justify-between w-full h-24 mx-auto font-medium md:justify-center"
        >
          <a href="#_" class="w-1/4 py-4 pl-6 pr-4 md:pl-4 md:py-0">
            <span
              class="p-1 text-xl font-black leading-none text-white select-none"
              ><span>A.l.y.s.u.m</span
              ><span class="text-gray-900">.</span></span
            >
          </a>
          <div
            class="fixed top-0 left-0 z-40 items-center w-full h-full p-3 text-xl bg-gray-900 bg-opacity-50 md:text-sm lg:text-base md:w-3/4 md:bg-transparent md:p-0 md:relative md:flex"
            v-if="showMenu === true"
          >
            <div
              class="flex-col w-full h-[70vh] bg-white rounded-lg select-none md:bg-transparent md:rounded-none md:relative md:flex md:flex-row md:overflow-auto"
            >
              <div
                class="flex flex-col items-center justify-center w-full h-full mt-12 text-center text-gray-900 md:text-gray-400 md:w-2/3 md:mt-0 md:flex-row md:items-center"
              >
                <a
                  href="#"
                  class="inline-block px-4 py-2 mx-2 font-medium text-left text-gray-900 md:text-white md:px-0 lg:mx-3 md:text-center"
                  >Home</a
                >
                <a
                  href="#"
                  class="inline-block px-0 px-4 py-2 mx-2 font-medium text-left md:px-0 hover:text-gray-900 md:hover:text-white lg:mx-3 md:text-center"
                  >About Us</a
                >
                <a
                  href="#"
                  class="inline-block px-0 px-4 py-2 mx-2 font-medium text-left md:px-0 hover:text-gray-900 md:hover:text-white lg:mx-3 md:text-center"
                  >Roadmap</a
                >
              </div>
              <div
                class="flex flex-col items-center justify-end w-full h-full pt-4 md:w-1/3 md:flex-row md:py-0"
              >
                <a
                  href="https://discord.gg/BztazGcKW2"
                  class="w-full pl-6 mr-0 text-gray-500 hover:text-white md:pl-0 md:mr-3 lg:mr-5 w-auto"
                  >Discord</a
                >
                <a
                  href="https://docs.google.com/forms/d/1CLXQnJk6N05s1022hxj8r2ouZML7CcWIC61-P9nSOKw/viewform?edit_requested=true"
                  class="inline-flex items-center justify-center px-4 py-2 mr-1 text-base font-medium leading-6 text-gray-900 whitespace-no-wrap transition duration-150 ease-in-out bg-white border border-transparent rounded-full hover:bg-white focus:outline-none focus:border-gray-900 focus:shadow-gray-NaN active:bg-gray-900"
                  >Join Team</a
                >
              </div>
            </div>
          </div>
          <div
            @click="toggleMenu()"
            class="absolute right-0 z-50 flex flex-col items-end w-10 h-10 p-2 mr-4 rounded-full cursor-pointer md:hidden hover:bg-gray-900 hover:bg-opacity-10 text-gray-100"
          >
            <svg
              class="w-6 h-6"
              x-show="!showMenu"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path d="M4 6h16M4 12h16M4 18h16"></path>
            </svg>
            <svg
              class="w-6 h-6"
              x-show="showMenu"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
              style="display: none"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              ></path>
            </svg>
          </div>
        </div>
      </nav>
      <div class="container py-32 mx-auto text-center sm:px-4">
        <h1
          class="text-4xl font-extrabold leading-10 tracking-tight text-white sm:text-5xl sm:leading-none md:text-6xl xl:text-4xl"
        >
          <span class="block">Join our Game Development Journal</span>
          <span
            class="relative inline-block mt-3 text-transparent text-white headeranim"
            >Project: A.l.y.s.u.m</span
          >
        </h1>
        <div
          class="max-w-lg mx-auto mt-6 text-sm text-center text-gray-200 md:mt-12 sm:text-base md:max-w-xl md:text-lg xl:text-xl"
        >
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry. Lorem Ipsum has been the industry's standard dummy text ever
          since the 1500s, when an unknown printer took a galley of type and
          scrambled it to make a type specimen book. It has survived not only
          five centuries, but also the leap into electronic typesetting,
          remaining essentially unchanged. It was popularised in the 1960s with
          the release of Letraset sheets containing Lorem Ipsum passages, and
          more recently with desktop publishing software like Aldus PageMaker
          including versions of Lorem Ipsum
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      showMenu: true,
    }
  },
  methods: {
    toggleMenu() {
      this.showMenu = !this.showMenu
    },
  },
}
</script>

<style>
.headeranim {
  -webkit-animation: colorchange 20s infinite alternate;
}

@-webkit-keyframes colorchange {
  0% {
    color: rgb(53, 53, 250);
  }
  10% {
    color: #8e44ad;
  }
  20% {
    color: #1abc9c;
  }
  30% {
    color: #d35400;
  }
  40% {
    color: rgb(57, 57, 214);
  }
  50% {
    color: #34495e;
  }
  60% {
    color: rgb(75, 75, 196);
  }
  70% {
    color: #2980b9;
  }
  80% {
    color: #f1c40f;
  }
  90% {
    color: #2980b9;
  }
  100% {
    color: pink;
  }
}
</style>
