<template>
  <v-container>
    <v-row align="center" class="row--35">
      <v-col lg="5" md="5" cols="12">
        <div class="thumbnail">
          <slot name="thum-img">words</slot>
        </div>
      </v-col>
      <v-col lg="7" md="7" cols="12">
        <div class="about-inner inner">
          <div class="section-title">
            <h2 class="heading-title">About Me</h2>
            <p class="description">
              I am a Frontend Developer who is passionate about building great user experiences. I am ambitious and user-focused with experience working not only in teams but independently.
            </p>
            <p class="description">  I have strong project management experience and experience delegating responsibilities to a team. A flexible and a quick learner committed to constantly learning and evolving my skills I try to stay abreast of ever-evolving technologies and trends in the industry.
            </p>           
            <p class="description">Communicative, knowledgeable and steadfast with excellent computer engineering skills. HTML5, CSS,JavaScript, VueJS, and ReactJS. When I'm not coding, you'll find me baking delicous desserts.
            </p>
          </div>
          <v-row class="mt--30 mt_sm--10">
            <v-col lg="6" md="6" sm="12" cols="12">
              <div class="about-us-list">
                <h3 class="heading-title">
                  Who we are
                </h3>
                <p>
                  There are many vtions of passages of Lorem Ipsum available,
                  but the majority have suffered.
                </p>
              </div>
            </v-col>
            <v-col lg="6" md="6" sm="12" cols="12">
              <div class="about-us-list">
                <h3 class="heading-title">
                  Who we are
                </h3>
                <p>
                  There are many vtions of passages of Lorem Ipsum available,
                  but the majority have suffered.
                </p>
              </div>
            </v-col>
          </v-row>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
