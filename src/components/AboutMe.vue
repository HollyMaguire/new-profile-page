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
          I am most comfortable with JavaScript with React or Vue. I am also good with Angular and typescript, I can use HTML (which I think pretty much anyone can), Css, Vuetify, Bootstrap, BootstrapVue. I also know Python with Django, and Ruby on Rails. I have used AWS in the past as well as Heroku and Docker. My experience using AWS has been with EC2, RDS, S3 buckets, AWS Lambda function, SNS Topics, Route 53, RDS, SES, SNS, load balancing and auto scaling. As well as Object Storage Options and Monitoring Services.

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
