<template>
  <div>
    <v-navigation-drawer
      class="hidden-md-and-up header-one-page-nav-drawer"
      v-model="drawer"
      fixed
      width="320"
    >
      <v-list-item class="pa-5">
        <div class="logo">
          <img
            src=../../assets/images/logo/s_thumbnail_header.png
            alt="S Logo"
          />
        </div>
        <v-spacer></v-spacer>
        <v-btn
          class="close-icon"
          icon
          @click="drawer = !drawer"
          v-html="iconSvg(closeIcon)"
        >
        </v-btn>
      </v-list-item>
      <scrollactive
        active-class="v-btn--active"
        bezier-easing-value=".5,0,.35,1"
        :offset="71"
      >
        <v-list>
          <v-list-item
            :ripple="false"
            v-for="item in items"
            :key="item.title"
            :to="item.to"
            link
            class="scrollactive-item"
          >
            <v-list-item-content>
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <!-- End mobile menu sidebar item list -->
        </v-list>
      </scrollactive>
    </v-navigation-drawer>
    <!-- End sidebar mobile menu -->

    <v-app-bar
      dark
      color="transparent"
      fixed
      elevate-on-scroll
      class="header-one-page-nav"
    >
      <router-link to="/" class="logo">
        <slot name="logo"></slot>
        <slot name="logo-dark"></slot>
      </router-link>
      <!-- End brand logo -->
      <v-spacer></v-spacer>
      <v-btn
        icon
        class="ma-0 pa-0 hidden-md-and-up"
        @click="drawer = !drawer"
        v-html="iconSvg(icon)"
      >
      </v-btn>
      <!-- End mobile menu icon -->
      <v-toolbar-items class="hidden-xs-only hidden-sm-only height-auto">
        <scrollactive
          active-class="v-btn--active"
          bezier-easing-value=".5,0,.35,1"
          :offset="71"
        >
          <v-btn
            v-for="item in items"
            :key="item.title"
            :to="item.to"
            link
            :ripple="false"
            text
            class="scrollactive-item"
            >{{ item.title }}</v-btn
          >
        </scrollactive>

        <a
          class="rn-btn"
          href="https://themeforest.net/checkout/from_item/30195230?license=regular"
        >
          <span>buy now</span>
        </a>
      </v-toolbar-items>
      <!-- End header menu item -->
    </v-app-bar>
    <!-- End top header navbar -->
  </div>
</template>

<script>
import feather from "feather-icons";
export default {
  data: () => ({
    drawer: false,
    items: [
      { title: "Home", to: "#home" },
      { title: "Service", to: "#service" },
      { title: "Get Start", to: "#getstart" },
      { title: "About", to: "#about" },
      { title: "Team", to: "#team" },
      { title: "Testimonial", to: "#tesimonial" },
      { title: "Portfolio", to: "#portfolio" },
    ],
    icon: "menu",
    closeIcon: "x",
  }),
  methods: {
    iconSvg(icon) {
      return feather.icons[icon].toSvg();
    },
  },
};
</script>
