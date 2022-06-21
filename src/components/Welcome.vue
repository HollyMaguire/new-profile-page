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
        <!-- <base-bubble-1
          style="transform: rotate(180deg) translateY(25%)"
        /> -->

        <v-row
          align="center"
          justify="center"
        >
          <v-col
            cols="10"
            md="6"
          >
        <base-heading class="info--text">
             Code challenges and assessments samples
            </base-heading>
            <base-text>
            I linked a page with little games and tools that I have noticed are commonly asked for in coding assessments I also have <a href="https://github.com/HollyMaguire"> <strong> My Git Hub link</strong></a>
            Included. On Github I have public projects in JavaScript, Python and Ruby. Many of the public ones are also previous assessments. I have included links to other past assessments for easier viewing. I also have aditional samples of my work below this section.
            </base-text>
               <base-btn class="mt-4">
               <a href="https://git-lab-challenge.herokuapp.com/">Searches through a gitlab project and uses GraphQl </a>
            </base-btn>
              <base-btn class="mt-4">
               <a href="https://gentle-sierra-10626.herokuapp.com/#/Memory">Games and commonly asked task/assessments</a>
            </base-btn>
             <base-text class="mb-5">On CodePen </base-text>
               <base-btn class="mt-4">
               <a href="https://codepen.io/hollyMaguire/pen/gOvJNJd">Select a user and see all of their post</a>
            </base-btn>
               <base-btn class="mt-4">
               <a href="https://codepen.io/hollyMaguire/pen/ZEemarz">Tic-tac-toe</a>
            </base-btn>
            <br>
              <base-btn class="mt-4">
               <a href="https://codepen.io/hollyMaguire/pen/zYNeExx">User list</a>
            </base-btn>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </section>
</template>
