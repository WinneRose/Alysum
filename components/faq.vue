<template>
  <div>
    <section class="text-gray-700">
      <div class="container px-5 py-24 mx-auto bg-[#16161a]">
        <div class="text-center mb-20 headeranim">
          <h1
            class="sm:text-3xl text-2xl font-medium text-center title-font mb-4"
          >
            Frequently Asked Question
          </h1>
          <p class="text-base leading-relaxed xl:w-2/4 lg:w-3/4 mx-auto">
            The most common questions about how our business works and what can
            do for you.
          </p>
        </div>
        <div class="flex flex-wrap lg:w-4/5 sm:mx-auto sm:mb-2 -mx-2">
          <div class="w-full lg:w-1/2 px-4 py-2">
            <details class="mb-4">
              <summary class="font-semibold mBg rounded-md py-2 px-4">
                How Long is this site live?
              </summary>

              <span class="text-gray-200">
                Laboris qui labore cillum culpa in sunt quis sint veniam. Dolore
                ex aute deserunt esse ipsum elit aliqua. Aute quis minim velit
                nostrud pariatur culpa magna in aute.
              </span>
            </details>
            <details class="mb-4">
              <summary class="font-semibold mBg rounded-md py-2 px-4">
                Can I install/upload anything I want on there?
              </summary>

              <span class="text-gray-200">
                Laboris qui labore cillum culpa in sunt quis sint veniam. Dolore
                ex aute deserunt esse ipsum elit aliqua. Aute quis minim velit
                nostrud pariatur culpa magna in aute.
              </span>
            </details>
            <details class="mb-4">
              <summary class="font-semibold mBg rounded-md py-2 px-4">
                How can I migrate to another site?
              </summary>

              <span class="text-gray-200">
                Laboris qui labore cillum culpa in sunt quis sint veniam. Dolore
                ex aute deserunt esse ipsum elit aliqua. Aute quis minim velit
                nostrud pariatur culpa magna in aute.
              </span>
            </details>
          </div>
          <div class="w-full lg:w-1/2 px-4 py-2">
            <details class="mb-4">
              <summary class="font-semibold mBg rounded-md py-2 px-4">
                Can I change the domain you give me?
              </summary>

              <span class="px-4 py-2 text-gray-200">
                Laboris qui labore cillum culpa in sunt quis sint veniam. Dolore
                ex aute deserunt esse ipsum elit aliqua. Aute quis minim velit
                nostrud pariatur culpa magna in aute.
              </span>
            </details>
            <details class="mb-4">
              <summary class="font-semibold mBg rounded-md py-2 px-4">
                How many sites I can create at once?
              </summary>

              <span class="px-4 py-2 text-gray-200">
                Laboris qui labore cillum culpa in sunt quis sint veniam. Dolore
                ex aute deserunt esse ipsum elit aliqua. Aute quis minim velit
                nostrud pariatur culpa magna in aute.
              </span>
            </details>
            <details class="mb-4">
              <summary class="font-semibold mBg rounded-md py-2 px-4">
                How can I communicate with you?
              </summary>

              <span class="px-4 py-2 text-gray-200">
                Laboris qui labore cillum culpa in sunt quis sint veniam. Dolore
                ex aute deserunt esse ipsum elit aliqua. Aute quis minim velit
                nostrud pariatur culpa magna in aute.
              </span>
            </details>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {}
</script>

<style>
.headeranim {
  -webkit-animation: colorchange 20s infinite alternate;
}

.mBg {
  background-color: rgba(63, 71, 82, 0.692);
  color: whitesmoke;
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
