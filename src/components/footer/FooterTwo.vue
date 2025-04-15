<template>
  <!-- Start Footer Style Two  -->
  <div
    class="footer-style-2 ptb--30 bg_image bg_image--1"
    data-black-overlay="6"
  >
    <div class="wrapper plr--50 plr_sm--20">
      <v-row align="center">
        <v-col lg="4" md="4" sm="6" cols="12">
          <div class="inner">
            <div class="logo text-center text-sm-left mb_sm--20">
              <router-link to="/"
                ><img :src="logo" alt="Logo images"
              /></router-link>
            </div>
          </div>
        </v-col>
        <!-- End .col -->
        <v-col lg="4" md="4" sm="6" cols="12">
          <div class="inner text-center">
            <ul class="social-share rn-lg-size d-flex justify-center liststyle">
              <li v-for="(social, i) in socialList" :key="i">
                <a target="_blank" :href="social.url"
                  ><i class="fab" :class="social.icon"></i
                ></a>
              </li>
            </ul>
          </div>
        </v-col>
        <!-- End .col -->
        <v-col lg="4" md="4" sm="12" cols="12">
          <div class="inner text-md-right text-center mt_md--20 mt_sm--20">
            <div class="text">
              <p>
                Copyright © {{ new Date().getFullYear() }} Sulai Sivadel. All
                Rights Reserved.
              </p>
            </div>
          </div>
        </v-col>
        <!-- End .col -->
      </v-row>
    </div>
  </div>
  <!-- End Footer Style Two  -->
</template>

<script>
  export default {
    data() {
      return {
        logo: require("../../assets/images/logo/apple-touch-icon.png"),
        socialList: [
          {
            icon: "fa-linkedin-in",
            url: "https://www.linkedin.com/in/sulai3030/",
          },
          {
            icon: "fa-bluesky",
            url: "https://bsky.app/profile/sulai3030.bsky.social",
          },
          {
            icon: "fa-instagram-square",
            url: "https://www.instagram.com/sulai3030/",
          },
        ],
      };
    },
  };
</script>
