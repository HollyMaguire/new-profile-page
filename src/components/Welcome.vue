<template>
  <section
    id="welcome"
    class="overflow-hidden"
  >
    <v-row no-gutters>
      <v-col
        class="hidden-sm-and-down"
        md="6"
      >
        <v-img
          :src="require('@/assets/cartmanOnComputer.jpg')"
          height="100vh"
        />
      </v-col>

      <v-col
        class="align-content-space-between layout wrap"
        cols="12"
        md="6"
        :pa-5="$vuetify.breakpoint.smAndDown"
      >
        <base-bubble-1
          style="transform: rotate(180deg) translateY(25%)"
        />

        <v-row
          align="center"
          justify="center"
        >
          <v-col
            cols="10"
            md="6"
          >
            <base-text>I linked a little projects page with little games and tools in the button below. I also have <a href="https://github.com/HollyMaguire"> <strong> My Git Hub link</strong></a>
Included. On Github I have projects in JavaScript, Python and Ruby. I did a coding bootcamp and I contunue to learn on my own.I know JavaScript, Python, HTML, CSS and Vue and I am learning Ruby on Rails currently. I have done some contract work with a backend engineer, doing the front-end parts of applications to make internal tools.
            </base-text>
            <base-btn class="mt-4">
              See Projects
            </base-btn>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </section>
</template>
