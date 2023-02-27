<template>
  <div>
    <!-- Start Header Area -->
    <Header>
      <img slot="logo" src="../../assets/images/logo/s_thumbnail_header.png" />
    </Header>
    <!-- End Header Area -->

    <!-- Start Breadcrump Area  -->
    <div
      class="rn-page-title-area pt--120 pb--190"
      data-black-overlay="20"
    >
      <v-container>
        <v-row>
          <v-col cols="12">
            <div class="rn-page-title text-center pt--100">
              <h2 class="headingtitle theme-gradient">Website Development & Professional Writing Services</h2> 
              <p class="text-center">I develop and maintain user oriented websites, and write and edit content as well </p>
            </div>
            <p></p>
            <p></p>
                <v-btn
                      a @click="$vuetify.goTo('#healthcare', options)"
                      color="#F42D2D"
                      elevation="24"
                      large
                      raised
                      rounded
                    >Healthcare Copywriting
                </v-btn> 
                &nbsp;
                <v-btn 
                      a @click="$vuetify.goTo('#policy', options)"
                      color="#F42D2D"
                      elevation="24"
                      large
                      raised
                      rounded> Healthcare Policy and Writing
                </v-btn>
                &nbsp;
                <v-btn
                     a @click="$vuetify.goTo('#technical', options)"
                      color="#F42D2D"
                      elevation="24"
                      large
                      raised
                      rounded
                    >Technical Writing
                </v-btn>
                &nbsp;
                <v-btn
                    a @click="$vuetify.goTo('#criticism', options)"
                     color="#F42D2D"
                      elevation="24"
                      large
                      raised
                      rounded>Film and TV Criticism
                </v-btn> 
          </v-col>
        </v-row>
      </v-container>
    </div>
    <!-- End Breadcrump Area  -->

    <div class="rn-service-details rn-section-gap bg_color--1">
      <v-container>
        <v-row>
          <v-col lg="12">
            <div class="service-details-inner">
              <div class="inner">
                <!-- Start Single Content  -->
                <v-row
                  class="sercice-details-content pb--80 align-items-center"
                >
                  <v-col lg="6" md="6" cols="12">
                    <div class="thumb">
                      <img
                        class="w-100"
                        src="https://i.imgur.com/3Jgb7lr.jpg"
                        alt="Service Images"
                      />
                    </div>
                  </v-col>
                  <v-col lg="6" md="6" cols="12">
                    <div class="details mt_md--30 mt_sm--30">
                      <h4 class="title theme-gradient">
                        <p>
                          Web Design and Development
                        </p>
                      </h4>
                      <p>
                        From conception to launch, from wireframe to testing I will dutifully complete and maintain your website.
                      </p>
                      <p>
                        Below are links to, and screenshots of, satified custormers' websites.
                      </p>
                      <h4 class="title"></h4>
                      <ul class="liststyle bullet">
                        <li><a href="https://web.archive.org/web/20220707140808/https://partydash.com/">PARTYDASH.COM</a></li>
                        <li><a href="https://www.mayapplecenter.org/">Mayapple Center for the Arts</a></li>
                        <li><a href="https://www.johndavidwest.com/">John David West: Social Media + Photography</a></li>
                        <li><a href="https://nymedicaidchoice.com/">New York Medicaid Choice by Maxim</a></li>
                        <li><a href="https://www.princetonreview.com/law-school-advice/strategies-to-succeed">The Princeton Review</a></li>
                      </ul>
                    </div>
                  </v-col>
                </v-row>
                <!-- End Single Content  -->
                <!-- Start Single Content  -->
                <v-row class="sercice-details-content align-items-center">
                  <v-col lg="6" md="6" cols="12" order="2" order-md="1">
                    <div class="details mt_md--30 mt_sm--30">
                      <h4 class="title">My Working Process</h4>
                      <ul class="liststyle bullet">
                        <li>My process is simple:</li>
                        <li>I meet with a client and discuss their needs.</li>
                        <li>Then I create a mockup of what I interpret from that conversation.</li>
                        <li>Receive feedback from client</li>
                        <li>Test vigoursly.</li>
                        <li> Launch site.</li>
                      </ul>
                    </div>
                  </v-col>
                  <v-col lg="6" md="6" cols="12" order="1" order-md="2">
                    <div class="thumb position-relative">
                      <img src="https://i.imgur.com/eOpUn1T.png"/>
                      <div class="thumbnail position-relative">
                        <div class="thumb"></div>
                      </div>
                    </div>
                  </v-col>
                </v-row>
                <!-- End Single Content  -->
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
     <div class="rn-service-details-health rn-section-gap bg_color--1">
      <v-container>
        <v-row>
          <v-col lg="12">
            <div class="service-details-inner">
              <div class="inner">
                <!-- Start Single Content  -->
                <v-row
                  class="sercice-details-content pb--80 align-items-center"
                >
                  <v-col lg="6" md="6" cols="12">
                    <div class="thumb">
                      <img
                        class="w-100"
                        src="https://i.imgur.com/OqgKnXy.jpg"
                        alt="Service Images"
                      />
                    </div>
                  </v-col>
                  <v-col lg="6" md="6" cols="12">
                    <div class="details mt_md--30 mt_sm--30">
                      <h4 class="headingtitle theme-gradient">
                       <p class="text-center" id="healthcare">Healthcare Copy Writing</p>
                      </h4>
                      <p>
                        I have written extensively in the healthcare realm. My writings include articles, and interviews with subject matter experts (SMEs
                      </p>
                      <p>Here are examples of my work.</p>
                      <ul class="liststyle bullet">
                        <li><a href="https://blackhealthmatters.com/lauren-lee-talks-kidney-disease-breakthroughs/">Lauren Lee talks kidney disease breakthroughs</a></li>
                        <li><a href="https://blackhealthmatters.com/is-there-a-light-at-the-end-of-the-dark-tunnel-of-kidney-disease-in-children/">Is there light at the end of the tunnel of kidney    Disease? An interview with Dr. Gbadegesin </a></li>
                        <li><a href="https://blackhealthmatters.com/working-with-your-doctor-when-you-have-kidney-disease-empowering-yourself-to-be-an-advocate-for-you">Working with your doctor. Empowering Yourself to be an Advocate for Yourself</a></li>
                        <li><a href="https://blackhealthmatters.com/kidney-disease/what-is-fsgs/">What is FSGS?</a></li>
                        <li><a href="https://blackhealthmatters.com/kidney-disease/truth-about-chronic-kidney-disease/">The Truth About Kidney Disease.</a></li>
                        <li><a href="https://blackhealthmatters.com/clinical-trials/how-can-i-find-a-clinical-trial/">How Can I Be In A Clinical Trial?</a></li>
                      </ul>
                    </div>
                  </v-col>
                </v-row>
                <!-- End Single Content  -->

                <!-- Start Single Content  -->
                <v-row class="sercice-details-content align-items-center">
                  <v-col lg="6" md="6" cols="12" order="2" order-md="1">
                    <div class="details mt_md--30 mt_sm--30">
                      <h4 class="headingtitle theme-gradient">Health Policy Writing and Reporting</h4>
                      <p id="policy">I have also edited and written healthcare policy for official websites such as this one for the State of New York touting the roll-out of a new health insurance plan for the disabled population. New York Medicaid Choice is the managed care enrollment program of the New York State Department of Health.</p>
                      <ul class="liststyle bullet">
                        <li><a href="https://nymedicaidchoice.com//">New York Medicaid Choice.com</a></li>
                      </ul>
                    </div>
                  </v-col>
                  <v-col lg="6" md="6" cols="12" order="1" order-md="2">
                    <div class="thumb position-relative">
                      <img src="https://i.imgur.com/8Jk5vIg.jpg"/>
                      <div class="thumbnail position-relative">
                        <div class="thumb"></div>
                      </div>
                    </div>
                  </v-col>
                </v-row>
                <!-- End Single Content  -->
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="rn-service-details-health rn-section-gap bg_color--1">
      <v-container>
        <v-row>
          <v-col lg="12">
            <div class="service-details-inner">
              <div class="inner">
                <!-- Start Single Content  -->
                <v-row
                  class="sercice-details-content pb--80 align-items-center"
                >
                  <v-col lg="6" md="6" cols="12">
                    <div class="thumb">
                      <img
                        class="w-100"
                        src="https://imgur.com/04qJ5PF.jpg"
                        alt="Street at Sunset"
                      />
                    </div>
                  </v-col>
                  <v-col lg="6" md="6" cols="12">
                    <div class="details mt_md--30 mt_sm--30">
                      <h4 class="headingtitle theme-gradient">Technical Writing</h4>
                      <p id="technical">
                        I am also a technincal writer having written for the New York City Department of Bulidings when they digitized the process by which building owners register to build new, or improve upon existing, structures in the city of New York.
                      </p>
                      <ul class="liststyle bullet">
                        <li><a href="https://a810-dobnow.nyc.gov/publish/Index.html#!/">New York City Dept. of Buildings </a></li>
                      </ul>
                    </div>
                  </v-col>
                </v-row>
                <!-- End Single Content  -->

                <!-- Start Single Content  -->
                <v-row class="sercice-details-content align-items-center">
                  <v-col lg="6" md="6" cols="12" order="2" order-md="1">
                    <div class="details mt_md--30 mt_sm--30">
                      <h4 class="headingtitle theme-gradient">Film Reporting and Criticism</h4>
                      <ul class="liststyle bullet">
                       <p class="text-left" id="criticism">For years I wrote Film and TV reviews. Samples can be found here:</p>
                       <p class="text-left"><a href="https://screenrant.com/author/sulai/">https://screenrant.com/author/sulai/</a></p>
                       <p class="text-left"></p> 
                       <p class="text-left"><a href="https://screenrant.com/author/sulai/"></a></p>
                      </ul>
                    </div>
                  </v-col>
                  <v-col lg="6" md="6" cols="12" order="1" order-md="2">
                    <div class="thumb position-relative">
                      <img src="https://i.imgur.com/myoXfGB.jpg"/>
                      <div class="thumbnail position-relative">
                        <div class="thumb"></div>
                      </div>
                    </div>
                  </v-col>
                </v-row>
                <!-- End Single Content  -->
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <Footer />
  </div>
</template>

<script>
  import Header from "../../components/header/Header";
  import Footer from "../../components/footer/Footer";
  export default {
    components: {
      Header,
      Footer,
    },
    data() {
      return {
        items: [
          {
            thumb: require("../../assets/images/service/service-02.png"),
            src: "https://i.imgur.com/RuBhh5y.jpg",
          },
        ],
        index: null,
      };
    },
    data: () => ({
      showMenu: false,
      items: [
        { title: 'Heathcare Copy Writing' },
        { title: 'Healthcare Policy Writing and Reporting' },
        { title: 'Technical Writing' },
        { title: 'Film and TV Criticism' },
      ],
    }),
    methods: {},
  };
</script>
