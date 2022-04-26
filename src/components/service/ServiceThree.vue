<template>
  <div class="row mt_dec--30">
    <!-- Start Single Service  -->
    <v-col
      lg="4"
      md="4"
      sm="6"
      cols="12"
      class="mt--30"
      v-for="(service, i) in serviceContent"
      :key="i"
    >
      <div class="single-service service__style--2 bg-color-gray">
        <router-link to="/service-details">
          <div class="service">
            <div class="icon">
              <div v-html="iconSvg(service.icon)"></div>
            </div>
            <div class="content">
              <h3 class="heading-title">{{ service.title }}</h3>
              <p>
                {{ service.desc }}
              </p>
            </div>
          </div>
        </router-link>
      </div>
    </v-col>
    <!-- End Single Service  -->
  </div>
</template>

<script>
  import feather from "feather-icons";
  export default {
    data() {
      return {
        serviceContent: [
          {
            icon: "layers",
            title: "Website Development",
            desc: `I build appications with one simple goal in mind, to help users find what they need quickly and to ensure the site owner is satisfied.`,
          },
          {
            icon: "monitor",
            title: "Health and Wellness Writing",
            desc: `Conveying health info in a user friendly and inviting manner can be difficult, but I take great pride in ameliorating that pain point.`,
          },
          {
            icon: "monitor",
            title: "Health Policy Writing/Reporting",
            desc: `Conveying information to the public can be complicated but I take great care in simplifiying that process and helping the average citizen to understand what is happening around them.`,
          },
          {
            icon: "layers",
            title: "Technical Writing",
            desc: `As a technical Writer for the New York City Department of Buildings I collaborated with my team in translating all of the information that owners of buildings in NYC needed to a digital platform.`,
          },
          {
            icon: "monitor",
            title: "Film Criticism & Reporting",
            desc: `Writing for numerous outposts and delivering breaking news about Hollywood releases.`,
          },
        ],
        items: [
        { title: 'Click Me' },
        { title: 'Click Me' },
        { title: 'Click Me' },
        { title: 'Click Me 2' },
      ],
      };
    },
    methods: {
      iconSvg(icon) {
        return feather.icons[icon].toSvg();
      },
    },
  };
</script>
