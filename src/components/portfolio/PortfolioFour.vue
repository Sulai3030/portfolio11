<template>
  <v-row>
    <!-- Start Single Portfolio  -->
    <v-col
      lg="4"
      md="4"
      sm="6"
      cols="12"
      class="mt--40"
      v-for="(item, i) in portfolioContent"
      :key="i"
    >
      <div class="portfolio">
        <div class="thumbnail-inner">
          <v-img class="thumbnail" :src="item.src"></v-img>
          <v-img class="bg-blr-image" :src="item.src"></v-img>
        </div>
        <div class="content">
          <div class="inner">
            <p>{{ item.meta }}</p>
            <h4>
              <router-link to="portfolio-details">{{ item.title }}</router-link>
            </h4>
          </div>
        </div>
      <div>
        <div class="text-center">
           <v-btn
            rounded
            color="#cc225a"
            dark
          >
            More info
          </v-btn>
        </div>
      </div>
    </v-col>
    <!-- End Single Portfolio  -->
  </v-row>
</template>

<script>
  export default {
    data() {
      return {
        portfolioContent: [
          {
            src: require("../../assets/images/portfolio/pexels-ylanite-koppens-3123915.jpg"),
            meta: "Web Development",
            title: "Party Dash",
          },
          {
            src: require("../../assets/images/portfolio/grounds-landscape_port.jpg"),
            meta: "Web Development",
            title: "Mayapple Center for the Arts and Humanities",
          },
          {
            src: require("../../assets/images/portfolio/dave_headshot_04_12_22.jpg"),
            meta: "Web Development",
            title: "John David West, Social Media Manager",
          },
          {
            src: require("../../assets/images/portfolio/slater01.jpg"),
            meta: "Web Development",
            title: "Michelle Slater, PhD.",
          },
          {
            src: require("../../assets/images/portfolio/pexels-ekaterina-bolovtsova-5263829.jpg"),
            meta: "Web Development/QA",
            title: "The G.O.A.T. Voter App",
          },
          {
            src: require("../../assets/images/portfolio/pexels-cottonbro-7579831.jpg"),
            meta: "QA",
            title: "New York Medicaid Choice",
          },
        ],
      };
    },
  };
</script>
