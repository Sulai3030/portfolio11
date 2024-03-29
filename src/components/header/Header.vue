<template>
  <div>
    <v-navigation-drawer
      class="hidden-md-and-up"
      v-model="drawer"
      absolute
      temporary
      width="320"
    >
      <v-list-item class="pa-5">
        <div class="logo">
          <img
            src="../../assets/images/logo/s_thumbnail_header.png"
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

      <v-list>
        <v-list-group
          v-for="item in homeVersionSidebarDropDownItems"
          :key="item.title"
          v-model="item.active"
        >
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title v-text="item.title"></v-list-item-title>
            </v-list-item-content>
          </template>

          <v-list-item
            link
            :ripple="false"
            v-for="child in item.items"
            :to="child.to"
            :key="child.title"
          >
            <v-list-item-content>
              <v-list-item-title v-text="child.title"></v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-group>
        <!-- End sidebar home dropdown item list -->

        <v-list-group
          v-for="item in servicesSidebarDropDownItems"
          :key="item.title"
          v-model="item.active"
        >
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title v-text="item.title"></v-list-item-title>
            </v-list-item-content>
          </template>

          <v-list-item
            link
            :ripple="false"
            v-for="child in item.items"
            :to="child.to"
            :key="child.title"
          >
            <v-list-item-content>
              <v-list-item-title v-text="child.title"></v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-group>
        <!-- End sidebar services dropdown item list -->

        <v-list-group
          v-for="item in pagesSidebarDropDownItems"
          :key="item.title"
          v-model="item.active"
        >
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title v-text="item.title"></v-list-item-title>
            </v-list-item-content>
          </template>

          <v-list-item
            link
            :ripple="false"
            v-for="child in item.items"
            :to="child.to"
            :key="child.title"
          >
            <v-list-item-content>
              <v-list-item-title v-text="child.title"></v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-group>
        <!-- End sidebar pages dropdown item list -->

        <v-list-group
          v-for="item in blocksSidebarDropDownItems"
          :key="item.title"
          v-model="item.active"
        >
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title v-text="item.title"></v-list-item-title>
            </v-list-item-content>
          </template>

          <v-list-item
            link
            :ripple="false"
            v-for="child in item.items"
            :to="child.to"
            :key="child.title"
          >
            <v-list-item-content>
              <v-list-item-title v-text="child.title"></v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-group>
        <!-- End sidebar block dropdown item list -->

        <v-list-item
          :ripple="false"
          v-for="item in items"
          :key="item.title"
          :to="item.to"
          link
        >
          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <!-- End mobile menu sidebar item list -->
      </v-list>
    </v-navigation-drawer>
    <!-- End sidebar mobile menu -->

    <v-app-bar
      dark
      elevation="0"
      color="transparent"
      absolute
      class="default-header"
    >
      <router-link to="/" class="logo">
        <slot name="logo"></slot>
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
        <v-menu
          open-on-hover
          bottom
          min-width="240"
          offset-y
          transition="scroll-y-reverse-transition"
        >
          <template v-slot:activator="{ on, attrs }">
            <v-btn :ripple="false" text v-bind="attrs" v-on="on">
              Home
            </v-btn>
          </template>

          <v-list>
            <v-list-item
              link
              v-for="(item, index) in HomeVerisiondropDownItems"
              :key="index"
              :to="item.to"
            >
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
        <!-- End Home variants dropdown -->
        <v-menu
          open-on-hover
          bottom
          min-width="240"
          offset-y
          transition="scroll-y-reverse-transition"
        >
          <template v-slot:activator="{ on, attrs }">
            <v-btn :ripple="false" text v-bind="attrs" v-on="on">
              Service
            </v-btn>
          </template>

          <v-list>
            <v-list-item
              link
              v-for="(item, index) in ServicesdropDownItems"
              :key="index"
              :to="item.to"
            >
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
        <!-- End Services dropdown -->
        <v-btn :ripple="false" text to="/about">About</v-btn>

        <v-menu
          open-on-hover
          bottom
          min-width="240"
          offset-y
          transition="scroll-y-reverse-transition"
        >
          <template v-slot:activator="{ on, attrs }">
            <v-btn :ripple="false" text v-bind="attrs" v-on="on">
              Pages
            </v-btn>
          </template>

          <v-list>
            <v-list-item
              link
              v-for="(item, index) in PagesdropDownItems"
              :key="index"
              :to="item.to"
            >
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
        <!-- End pages dropdown -->

        <v-menu
          min-width="240"
          open-on-hover
          bottom
          offset-y
          transition="scroll-y-reverse-transition"
        >
          <template v-slot:activator="{ on, attrs }">
            <v-btn text :ripple="false" v-bind="attrs" v-on="on">
              
            </v-btn>
          </template>

          <v-list>
            <v-list-item
              link
              v-for="(item, index) in blocksDropDownItems"
              :key="index"
              :to="item.to"
            >
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
        <!-- End blocks dropdown -->
        <v-btn :ripple="false" text to="/contact">Contact</v-btn>
        
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
      //{ title: "About", to: "/about" },
      { title: "Contact", to: "/contact" },
    ],
    HomeVerisiondropDownItems: [
      //{ title: "Personal Portfolio 02", to: "landing-personal-portfolio-02" },
      {
        title: "Sulai Sivadel: Web Developer",
        to: "/landing-personal-portfolio-02",
      },
    ],
    ServicesdropDownItems: [
      
      { title: "Service Details", to: "/service-details" },
    ],
    PagesdropDownItems: [
      { title: "Blog List", to: "/blog" },
      { title: "Blog Details", to: "/blog-details" },
      { title: "Service", to: "/service" },
      { title: "Service Details", to: "/service-details" },
      { title: "Personal Portfolio 02", to: "landing-personal-portfolio-02" },
     
      { title: "404 Page", to: "/404" },
    ],
    

    // Bellow mobile menu items
    homeVersionSidebarDropDownItems: [
      {
        items: [
          { title: "Main Demo", to: "/main-demo" },
          { title: "Main Demo Dark", to: "/main-demo-dark" },
          { title: "Creative Agency", to: "/creative-agency" },
          {
            title: "Creative Agency Landing",
            to: "/landing-creative-agency",
          },
          { title: "Personal Portfolio", to: "/persoanl-portfolio" },
          {
            title: "Personal Portfolio 02",
            to: "landing-persoanl-portfolio-02",
          },
          {
            title: "Personal Portfolio Landing",
            to: "/landing-persoanl-portfolio",
          },
          { title: "Designer Portfolio", to: "/designer-portfolio" },
          { title: "Creative Portfolio", to: "/creative-portfolio" },
          { title: "Business", to: "/business" },
          { title: "Digital Agency", to: "/digital-agency" },
          { title: "Minimal Portfolio", to: "/minimal-portfolio" },
          { title: "Studio Agency", to: "/studio-agency" },
          { title: "Home Particles", to: "/landing-home-particle" },
          { title: "Startup", to: "/startup" },
          { title: "Home Paralax", to: "/parallax-home" },
          { title: "Corporate Business", to: "/corporate-business" },
          { title: "Interactive Agency", to: "/interactive-agency" },
        ],
        title: "Home",
      },
    ],
    servicesSidebarDropDownItems: [
      {
        items: [
          { title: "Service", to: "/service" },
          { title: "Service Details", to: "/service-details" },
        ],
        title: "Service",
      },
    ],
    pagesSidebarDropDownItems: [
      {
        items: [
          { title: "Blog List", to: "/blog" },
          { title: "Blog Details", to: "/blog-details" },
          { title: "Service", to: "/service" },
          { title: "Service Details", to: "/service-details" },
          { title: "Portfolio", to: "/portfolio" },
          { title: "Portfolio Details", to: "/portfolio-details" },
          { title: "404 Page", to: "/404" },
        ],
        title: "Pages",
      },
    ],
    blocksSidebarDropDownItems: [
      {
        items: [
          { title: "Portfolio", to: "/portfolio" },
          { title: "Team", to: "/team" },
          { title: "Service", to: "/service" },
          { title: "Video Popup", to: "/video-popup" },
          { title: "Progressbar", to: "/progressbar" },
          { title: "Gallery", to: "/gallery" },
          { title: "Counters", to: "/counter" },
          { title: "Blog List", to: "/blog" },
          { title: "Client Logo", to: "/brand" },
          { title: "Contact Form", to: "/contact-form" },
          { title: "Columns", to: "/column" },
          { title: "Button", to: "/button" },
          { title: "List Style", to: "/list-style" },
          { title: "Testimonial", to: "/testimonial" },
          { title: "Accordion", to: "/accordion-with-tab" },
          { title: "Pricing Plan", to: "/pricing-plan" },
        ],
        title: "Block",
      },
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

<style lang="scss">
.feather-menu {
  color: #c6c9d8;
}
</style>
