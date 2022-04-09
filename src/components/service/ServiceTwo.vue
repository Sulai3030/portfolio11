<template>
  <!-- Start Service Area  -->
  <v-row class="service-one-wrapper">
    <!-- Start Single Service  -->
    <v-col
      lg="6"
      md="6"
      sm="6"
      cols="12"
      v-for="(service, i) in serviceContent"
      :key="i"
    >
      <div class="single-service service__style--4">
        <router-link to="/service-details">
          <div class="service">
            <div class="icon" v-html="iconSvg(service.icon)"></div>
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
  </v-row>
  <!-- Start Service Area  -->
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
            desc: ` I like to design user friendly Frontends ensuring they are ADA Complient`,
          },
          {
            icon: "cast",
            title: "Web Editing",
            desc: ` I throw myself down among the tall grass by the stream as I lie
                close to the earth.`,
          },
          {
            icon: "monitor",
            title: "Writing for the Web",
            desc: `I write evergreen copy that is engaging and search-engine optimized.`,
          },
          {
            icon: "monitor",
            title: "Technical Writing",
            desc: `I have experience writing techincal manuals and how-to's for large coporate entities such as the city of New York.`,
          },
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
