<template>
  <v-container>
    <v-row align="center" class="row--35">
      <v-col lg="5" md="5" cols="12">
        <div class="thumbnail">
          <slot name="thum-img"></slot>
        </div>
      </v-col>
      <v-col lg="7" md="7" cols="12">
        <div class="about-inner inner">
          <div class="section-title">
            <h2 class="heading-title">About Me</h2>
              <p class="description">
                I am a Frontend Developer who is passionate about building inviting user experiences. I am ambitious and user-focused with experience working not only in teams but independently.
              </p>
              <p class="description">  I have strong project management experience and experience delegating responsibilities to a team. A flexible and quick learner         
                committed to constantly learning and evolving my skills, I try to stay abreast of ever-evolving technologies and trends in the industry.
              </p>           
              <p class="description">Communicative, knowledgeable and steadfast with excellent computer engineering skills. HTML5, CSS,JavaScript, VueJS, and ReactJS. When I'm not coding, you'll find me baking delicous desserts.
             </p>
          </div>
        </div>
      </v-col>
    </v-row>    
  </v-container>
</template>
