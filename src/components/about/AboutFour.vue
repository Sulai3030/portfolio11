<template>
  <v-row class="row--35" align="center">
    <v-col lg="5" md="5" cols="12">
      <div class="thumbnail">
        <slot name="thum-img"></slot>
      </div>
    </v-col>
    <v-col lg="7" md="7" cols="12">
      <div class="about-inner inner pt--100 pt_sm--40 pt_md--40">
        <div class="section-title">
          <h2 class="heading-title">About Me</h2>
           <p class="description"> I am a Frontend Developer who is passionate about building great user experiences. I am ambitious and user-focused with experience working in teams as well as independently.</p> 
           <p class="description">I have strong project management experience and experience delegating responsibilities to a team.
              A flexible and quick learner, I am committed to constantly evolving my skillset. I try to stay abreast of ever-evolving technologies and trends in the industry. </p>
            <p class="description">Communicative, knowledgeable and steadfast with excellent computer engineering skills. HTML5, CSS,JavaScript, VueJS, and ReactJS. When I'm not coding, you'll find me baking delicous desserts.</p>
        </div>
        <!-- End .section-title -->
        <div class="tab-wrapper mt--30">
          <v-row>
            <TabTwo />
          </v-row>
        </div>
      </div>
    </v-col>
  </v-row>
</template>

<script>
  import TabTwo from "../../components/tabs/TabTwo";
  export default {
    components: { TabTwo },
    data() {
      return {};
    },
  };
</script>
