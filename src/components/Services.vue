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
              Background
            </base-heading>

            <base-text class="mb-5">
I was originally a Chemist, with several publications to my name and I programmed robots in my lab. This is where I first fell in love with programming. I have a lot of analytical skills from my time in research, it also honed skills for problem solving and critical thinking.
I was the project lead for a Malaria drug discovery project which allowed me to develop leadership skills. I gained experience working in teams from animal work project, all animal work was done closely with a team. I also have experience working independently from a cloning and gene-splicing project, and from my time doing polymer research.
In more recient years I have been switching to software and doing contract work, first with front end projects then transistioned into fullstack contracts. I am currently doing

            </base-text>
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
      services: [
        {
          name: 'Research',
          icon: 'mdi-clipboard-text-outline',
        },
        {
          name: 'Development',
          icon: 'mdi-settings-outline',
        },
      ],
    }),
  }
</script>
