<template>
  <section
    id="services"
    class="overflow-hidden"
  >
    <v-row
      class="accent"
      no-gutters
    >
      <v-col
        class="hidden-sm-and-down"
        md="6"
      >
        <v-img
          :src="require('@/assets/services.png')"
          height="100%"
        />
      </v-col>

      <v-col
        class="text-center pa-5"
        cols="12"
        md="6"
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <v-col cols="12">
            <base-bubble-2
              style="transform: translateX(55%)"
            />
            <base-heading class="info--text">
              Sample Work
            </base-heading>
            <base-text class="mb-5">The majority of my work is not visable to the public, but I have given external links for some parts of my work which can be publically viewed. For Fedmall only small parts are viewable for the public.
            </base-text>
            <base-btn class="mt-4">
               <a href="https://www.eia.gov/international/data/world">International Data</a>
            </base-btn>
                        <base-btn class="mt-4">
               <a href="https://www.eia.gov/todayinenergy/">Today in Energy</a>
            </base-btn>
                        <base-btn class="mt-4">
               <a href="https://www.fedmall.mil/index.html">FedMall</a>
            </base-btn>
                        <base-btn class="mt-4">
               <a href="https://www.eia.gov/outlooks/steo/">Short Term Energy Outlook</a>
            </base-btn>
                             <base-btn class="mt-4">
               <a href="https://www.eia.gov/opendata/">Open Data</a>
            </base-btn>
          </v-col>

          <v-col
            v-for="(service, i) in services"
            :key="i"
            class="text-center mb-3"
            md="6"
          >
            <v-avatar
              class="elevation-6 mb-2"
              color="#69A1BB"
              size="64"
              tile
            >
              <v-icon
                dark
                size="52"
                v-text="service.icon"
              />
            </v-avatar>

            <base-text>
              <div
                class="mb-2"
                v-text="service.name"
              />
              <div v-html="service.blurb" />
            </base-text>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </section>
</template>

<script>
  export default {
    name: 'Services',

    data: () => ({
      projects: [
        'https://www.eia.gov/international/data/world',
        'https://www.eia.gov/todayinenergy/',
        'https://www.fedmall.mil/index.html',
        'https://www.eia.gov/outlooks/steo/',
        'https://www.eia.gov/opendata/',
      ],
    }),
  }
</script>
