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
         I prefer front end engineering, but I have also worked in fullstack. For my start in software I was working various contracts mostly internal HR tools. I then went into government work, with the deapartment of energy/eia and the deparment of defense, modernizing fedmall. I have developed using Windows and Linux.
        </base-text>

        <base-subheading class="info--text">
          Skills
        </base-subheading>

        <base-text class="mb-5">
          Front-end: Vue, React, Angular, Javascript, Typescript, Scss, Css, Vuetify, Bootstrap, BootstrapVue, WAVE,  Scss, Css, HMTL <br>
          Back-end: Ruby on rails, Python, PHP<br>
          Dev-ops: EC2, RDS, S3, SNS, SES, Lambda, Elastic Beanstalk, VPC, IAM, AMI, Auto Scaling, Load Balancing, deployment with AWS.
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
