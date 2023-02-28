<template>
  <div class="active-dark">
    <!-- Start Header Area -->
    <HeaderOnePageTwo />
    <!-- End Header Area -->
    <!-- Start Slider Area  -->
    <div class="rn-slider-area poss_relative" id="home">
      <div
        class="slide personal-portfolio-slider slider-style-3 slider-paralax bg_image bg-image-8 d-flex align-center"
      >
        <BannerThree>
          <span slot="designation">Web Developer and Designer</span>
          <h2 class="heading-title" slot="heading-title">
            I am Sulai Sivadel. Welcome to my Portfolio.
          </h2>
        </BannerThree>
      </div>
    </div>
    <!-- End Slider Area -->

    <!-- Start About Area  -->
    <div class="section about-area rn-section-gap bg_color--1" id="about">
      <div class="about-wrapper">
        <div class="container">
          <AboutFour>
            <img
              slot="thum-img"
              class="w-100"
              src="../../assets/images/bg/sunset2.gif"
              alt="Winter Sunset"
            />
          </AboutFour>
        </div>
      </div>
    </div>
    <!-- Start About Area  -->

    <!-- Start Service Area  -->
    <div
      class="section service-area rn-service-area rn-section-gap bg_color--5"
      id="service"
    >
      <div class="container">
        <v-row>
          <v-col lg="12">
            <div
              class="section-title service-style--3 text-center mb--20 mb_sm--0 md_md--0"
            >
              <h2 class="heading-title">My Services</h2>
              <p class="text-left">
                I am passionate about building great and inviting user experiences. There is nothing better than a well contrsuctied and navigable website. My aim for you is to deliver that for you and your customers.
              </p>
            </div>
          </v-col>
        </v-row>
        <ServiceThree />
      </div>
    </div>
    <!-- Start Service Area  -->

    <!-- Start Portfolio Area -->
    <div
      class="section rn-portfolio-area rn-section-gap bg_color--1"
      id="portfolio"
    >
      <v-container>
        <v-row>
          <v-col lg="12">
            <div class="section-title section-title--2 text-center mb--20">
              <h2 class="heading-title">My Latest Projects</h2>
              <p class="text-left">
                I am user-focused and experienced with working in teams and independently. 
              </p>
              <p class="text-left">I have strong project management experience and experience 
                delegating responsibilities to a team. Bringing projects in on time and uneder budget.</p>
              <p class="text-left">A flexible and quick learner committed to constantly learning and evolving skills to stay abreast of ever-evolving technologies and trends in the industry. Communicative, knowledgeable and steadfast with excellent computer engineering skills. HTML5, CSS,JavaScript, VueJS, and ReactJS.
              When I'm not coding, you'll find me baking delicous desserts.
              </p>
            </div>
          </v-col>
        </v-row>
        <PortfolioFour />
        <v-row>
          <v-col lg="12">
            <div class="view-more-btn mt--60 mt_sm--30 text-center">
              <a class="rn-button-style--2 btn_solid" href="https://www.mayapplecenter.org">Mayapple Center for the Arts</a>&nbsp;
              <a class="rn-button-style--2 btn_solid" href="https://www.johndavidwest.com">John David West, Social Media Manager</a>&nbsp;
              <a class="rn-button-style--2 btn_solid" href="https://michelleslater.com/">Michelle Slater, PhD.</a>&nbsp;  
              <a class="rn-button-style--2 btn_solid" href="https://nymedicaidchoice.com/">State of New York, Medicaid Choice</a>&nbsp;
              <a class="rn-button-style--2 btn_solid" href="https://www.partydash.com">Party Dash (Archived Version)</a>&nbsp;
              <a class="rn-button-style--2 btn_solid" href="https://www.goatvoter.org/">The G.O.A.T. Voter App (Expired)</a>&nbsp;
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <!-- End Portfolio Area -->

    <!-- Start Blog Area  -->
    <div class="section rn-blog-area rn-section-gap bg_color--5" id="blog">
      <v-container>
        <v-row align="end" class="mb--20">
          <v-col lg="6" md="12">
            <div class="section-title text-left">
              <h2>Blog Posts</h2>
              <p>
                Below are some of the projects I am currently working on.
              </p>
            </div>
          </v-col>
        </v-row>
        <Blog />
      </v-container>
    </div>
    <!-- End Blog Area  -->

    <!-- Start Contact Area  -->
    <div
      class="section rn-contact-area rn-section-gap bg_color--1"
      id="contact"
    >
      <div class="contact-form--1">
        <v-container>
          <Contact>
            <img
              slot="contact-img"
              class="w-100"
              src="../../assets/images/portfolio/stormphoto.jpg"
              alt="storm"
              max-width="200"
              height="auto"
            />
          </Contact>
        </v-container>
      </div>
    </div>
    <!-- End Contact Area  -->

    <!-- Start Footer Area  -->
    <Footer />
    <!-- End Footer Area  -->
  </div>
</template>

<script>
import HeaderOnePageTwo from "../../components/header/HeaderOnePageTwo";
import BannerThree from "../../components/slider/BannerThree";
import AboutFour from "../../components/about/AboutFour";
import ServiceThree from "../../components/service/ServiceThree";
import PortfolioFour from "../../components/portfolio/PortfolioFour";
import Blog from "../../components/blog/Blog";
import Contact from "../../components/contact/Contact";
import Footer from "../../components/footer/FooterTwo";

export default {
  components: {
    HeaderOnePageTwo,
    BannerThree,
    AboutFour,
    ServiceThree,
    PortfolioFour,
    Blog,
    Contact,
    Footer,
  },
  data() {
    return {};
  },
};
</script>
