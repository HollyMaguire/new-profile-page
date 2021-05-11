<template>
  <section
    id="about"
    class="overflow-hidden"
  >
    <v-row
      class="white"
      no-gutters
    >
      <v-col
        class="pa-5"
        cols="12"
        md="6"
      >
        <base-bubble-1 style="transform: translate(5%, -5%)" />

        <base-heading class="info--text">
          About Me
        </base-heading>

        <base-text class="mb-5">
          <br>
        I love animals, I have a particular fondness of ducks, pidgeons and coy fish. I am a bjj blue belt, I also do judo and powerlifting.
        </base-text>

        <base-subheading class="info--text">
          Skills
        </base-subheading>

        <base-text class="mb-5">
          I am most comfortable with JavaScript using Vue as a framework. I can use HTML (which I think pretty much anyone can), Css, Vuetify, Bootstrap, BootstrapVue. I also know Python, and am learning Ruby on Rails currently. I have done a react and node class, as well as a Java with Springboot class. However these I did not list at the top of the site as I am not as comfortable with them but I could refresh them.
        </base-text>
      </v-col>

      <v-col
        class="hidden-sm-and-down"
        md="6"
      >
        <v-img
          :src="require('@/assets/aboutme.png')"
          height="100%"
        />
      </v-col>
    </v-row>
  </section>
</template>

<script>
  export default {
    data: () => ({
      skills: [
        {
          name: 'Web Design',
          value: 100,
        },
        {
          name: 'Web Development',
          value: 75,
        },
        {
          name: 'Web Support',
          value: 90,
        },
      ],
    }),
  }
</script>
