<template>
  <div class="flex items-center justify-center min-h-screen bg-gray-800 py-48">
    <div class="flex flex-col">
      <div class="flex flex-col mt-8">
        <!-- Meet the Team -->
        <div class="container max-w-7xl px-4">
          <!-- Section Header -->
          <div class="flex flex-wrap justify-center text-center mb-24">
            <div class="w-full lg:w-6/12 px-4">
              <!-- Header -->
              <h1 class="text-gray-200 text-4xl font-bold mb-8">
                Meet the Team
              </h1>

              <!-- Description -->
              <p class="text-gray-400 text-lg font-light">
                With over 100 years of combined experience, we've got a
                well-seasoned team at the helm.
              </p>
            </div>
          </div>

          <!-- Team Members -->
          <div class="flex flex-wrap">
            <!-- Member #1 -->
            <div
              class="w-full md:w-6/12 lg:w-3/12 mb-6 px-6 sm:px-6 lg:px-4"
              v-for="profiles in profile"
              :key="profiles"
            >
              <div class="flex flex-col">
                <!-- Avatar -->
                <a href="#" class="mx-auto">
                  <img
                    class="rounded-2xl drop-shadow-md hover:drop-shadow-xl transition-all duration-200 delay-100"
                    :src="profiles.img"
                  />
                </a>

                <!-- Details -->
                <div class="text-center mt-6">
                  <!-- Name -->
                  <h1 class="text-gray-200 text-xl font-bold mb-1">
                    {{ profiles.name }}
                  </h1>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      profile: [],
    }
  },

  async mounted() {
    const data = await this.$lanyard({
      userId: ['701896585604497490', '162969778699501569'],
    })
    //cdn.discordapp.com/avatars/701896585604497490/${status.discord_user.avatar}.png?size=256
    for (let i = 0; i < data.length; i++) {
      this.profile.push({
        img:
          'https://cdn.discordapp.com/avatars/' +
          `${data[i].data.discord_user.id}/` +
          data[i].data.discord_user.avatar +
          '.png?size=256',
        name: data[i].data.discord_user.username,
      })

      console.log(this.profile)
    }
  },
}

/*
  async mounted() {
    const socket = await this.$lanyard({
      userId: '701896585604497490',
      socket: true,
    })

    // Set a listener for "message" event
    socket.addEventListener('message', ({ data }) => {
      const { d: status } = JSON.parse(data)

      this.profileurl = `https://cdn.discordapp.com/avatars/701896585604497490/${status.discord_user.avatar}.png?size=256`
      this.name = status.discord_user.username
    })

    this.$lanyard({
      userId: ['162969778699501569', '94490510688792576'],
    })

    console.log(this.$lanyard)

    // Do whatever you want with Lanyard response object
  },*/
</script>

<style></style>
