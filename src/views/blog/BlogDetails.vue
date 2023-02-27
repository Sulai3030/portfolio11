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
      data-black-overlay="10"
    >
      <v-container>
        <v-row>
          <v-col cols="12">
            <div class="blog-single-page-title text-center pt--100">
              <h2 class="heading-title theme-gradient">
                Recent Posts<br />
              </h2>
              <ul class="blog-meta d-flex justify-center align-center">
                <li class="d-flex" v-for="(meta, i) in metaList" :key="i">
                  <span v-html="iconSvg(meta.icon)"></span>{{ meta.text }}
                </li>
              </ul>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <!-- End Breadcrump Area  -->

    <!-- Start Blog Details Area  -->
    <div class="rn-blog-details pt--110 pb--70 bg_color--1">
      <v-container>
        <v-row>
          <v-col cols="12">
            <div class="inner-wrapper">
              <div class="inner">
                <p>
                  <p>Burn Notice</p>
                  <p>Mid Season Premiere</p>
	                <p>The midseason premiere of Burn Notice begins with a voice over (VO) and collection of scenes of the previous season’s events. The VO used in Burn Notice is a quick way to bring new viewers up to date on the action that happens on the show from week to week as well as keeping returning viewers abreast after the midseason hiatus. Next, we receive a title card and freeze frames to provide info without the need for a voice over from the main character Michael Westen (Jeffrey Donovan).
                  </p>
                </p>
                <div class="thumbnail">
                  <img
                    src="../../assets/images/logo/pexels-obregonia-d-toretto-918281.jpg"
                    alt="Blog Images"
                    height="300"
                    width="150"
                  />
                </div>
                <p class="mt--40">
                  One of the signature tropes on Burn Notice is the VO. Burn Notice is a high concept show that attempts to relate the high stakes world of espionage in a very relatable manner and so unlike most lessons on screenwriting where you might be told that the use of VO is a failure by the screenwriter to convey information by showing the audience, Burn Notice uses VO as a tool to convey highly technical facts that would normally bog down the story. 
                </p>
                <p>
                  The show runners also use the VO to demonstrate how knowledgeable the main characters are of the world they inhabit.  These are professional spies. Burn Notice’s VO is a collaboration between the screenwriter and the director because the director frequently uses the VO in conjunction with aerial shots to change scenes and locations within the show itself. 
                </p>
                <blockquote class="rn-blog-quote"> </blockquote>
                <p>
                  Another thing that the VOs accomplish is to show what happens in subtext within a scene.  At the end of the first hour—this was a two-hour premiere— Madeline Westen, played by the incomparable (Sharon Gless), pretends as if she is a concerned mother worried about her son, while being questioned by Tom Card (John C. McGinley) while the VO tells us how someone who is trying to deceive another would act.   In reality she had already been in contact with her son.
                </p>
                <div class="blog-single-list-wrapper d-flex flex-wrap">
                  <div class="thumbnail">
                    <img
                      class="w-100"
                      src="../../assets/images/blog/52040863336_890ff8cd4d_e.jpg"
                      alt="BLog Images"
                    /><span
                      >Clouds after a storm</span
                    >
                  </div>
                  <div class="content">
                    <p>
                      The bridge between the two hours employs a device known as a reversal. In the first hour of the premiere, we have Westen and Tyler Grey (Kenny Johnson) captured by a Panamanian drug lord. In a surprise twist in the second hour, Tyler Gray shoots the Panamanian drug lord and tells Westen that he now believes everything Westen has been trying to explain for the past two episodes. This is called a reversal but it is also a good way to demonstrate character growth.
                    </p>
                  </div>
                </div>
                <p class="mt--25 mt_sm--5">
                  The second hour runs more like a typical episode of Burn Notice with the introduction of a character who needs assistance because she is being threatened with jail by a cop whose partner was shot by a drug dealer. Gabrielle Anwar’s character Fiona agrees to help the individual despite the protestations of the other members of the team. The VO in the second hour is very technical, all about the internal workings of the spy game, and contains a bit of foreshadowing. 
                </p>
                <div class="video-wrapper position-relative mb--40">
                  <div class="thumbnail">
                    <img
                      class="w-100"
                      src="../../assets/images/blog/52040863336_890ff8cd4d_e.jpg"
                      alt="BLog Images"
                      height="250"
                    width="150"
                    /><span
                      >Clouds after a storm</span
                    >
                  </div>
                  <div class="thumbnail position-relative">
                    <div v-for="(image, imageIndex) in items" :key="imageIndex">
                      <img
                        class="w-100"
                        :src="image.thumb"
                        alt="About Images"
                      />
                      <a
                        @click="index = imageIndex"
                        class="video-popup position-top-center play__btn"
                        ><span class="play-icon"></span
                      ></a>
                    </div>
                  </div>
                </div>
                <p class="mb--0">
                  The plot to the second episode bookends the burned spy arc and involves the aiding of a young mother in escaping harassment by a dirty cop.  But first the episode begins with the crew literally burning down their home base, which is possible foreshadowing for the rest of the season. It also contains a scene where Madeline confronts the man who killed her other son, Westen’s brother. This scene takes place on the waterfront; water is frequently a screenwriter’s go-to to demonstrate spiritual cleansing.
                </p>
                <p>The dialog playfully uses lyrics from the popular song “Public Service Announcement” by Jay-Z to punctuate explosions, a fun and cheeky way to bring in casual viewers. We are also given the cliché of the four main characters, Westen, Fiona, Sam Axe (Bruce Campbell), and Jesse Porter (Coby Bell) walking away from the scene in slow motion.</p>
                <p>
                 The dialog playfully uses lyrics from the popular song “Public Service Announcement” by Jay-Z to punctuate explosions, a fun and cheeky way to bring in casual viewers. We are also given the cliché of the four main characters, Westen, Fiona, Sam Axe (Bruce Campbell), and Jesse Porter (Coby Bell) walking away from the scene in slow motion.  
                </p>
                <p>We close out this storyline by showing the woman Fiona met in prison at the end of last season and subsequently aided, reunited with her son. The characters tell us through dialog that the issues that the woman Fiona was aiding were neatly resolved by a change of heart in the antagonist in the second episode. They don’t mention the gunplay or the explosions and the scene is light and played for light laughs.</p>
                <p>The final scene of the episode between Westen and his mother reveals her decision to go live with her sister and leave Miami but only after telling her son that he needs to retire after he accomplishes his goals of resolving his Burn Notice. This is a huge change as a major character now exits the show.</p>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <!-- End Blog Details Area  -->

    <!-- Start Comment Form  -->
    <div class="blog-comment-form pb--120 bg_color--1">
      <v-container>
        <v-row>
          <v-col cols="12">
            <div class="inner">
              <h3 class="title mb--40 fontWeight500">Leave a Reply</h3>
              <ValidationObserver v-slot="{ handleSubmit }">
                <form @submit.prevent="handleSubmit(onSubmit)">
                  <v-row>
                    <v-col lg="6" md="12" cols="12">
                      <div class="rnform-group">
                        <ValidationProvider
                          name="name"
                          rules="required"
                          v-slot="{ errors }"
                        >
                          <label>
                            <input
                              type="text"
                              v-model="formData.name"
                              placeholder="Name"
                            />
                            <span class="inpur-error">{{ errors[0] }}</span>
                          </label>
                        </ValidationProvider>
                      </div>
                      <div class="rnform-group">
                        <ValidationProvider
                          name="email"
                          rules="required|email"
                          v-slot="{ errors }"
                        >
                          <label>
                            <input
                              type="text"
                              rules="required|email"
                              v-model="formData.email"
                              placeholder="Email"
                            />
                            <span class="inpur-error">{{ errors[0] }}</span>
                          </label>
                        </ValidationProvider>
                      </div>
                      <div class="rnform-group">
                        <ValidationProvider
                          name="website"
                          rules="required"
                          v-slot="{ errors }"
                        >
                          <label>
                            <input
                              type="text"
                              v-model="formData.subject"
                              placeholder="Website"
                            />
                            <span class="inpur-error">{{ errors[0] }}</span>
                          </label>
                        </ValidationProvider>
                      </div>
                    </v-col>
                    <v-col lg="6" md="12" cols="12">
                      <div class="rnform-group">
                        <ValidationProvider
                          name="comment"
                          rules="required"
                          v-slot="{ errors }"
                        >
                          <label>
                            <textarea
                              v-model="formData.message"
                              placeholder="Comment"
                            ></textarea>
                            <span class="inpur-error">{{ errors[0] }}</span>
                          </label>
                        </ValidationProvider>
                      </div>
                    </v-col>
                    <v-col cols="12">
                      <div class="blog-submit-btn">
                        <button
                          class="rn-button-style--2 btn_solid"
                          type="submit"
                          value="submit"
                        >
                          SEND MESSAGE
                        </button>
                      </div>
                    </v-col>
                  </v-row>
                </form>
              </ValidationObserver>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <!-- End Comment Form  -->

    <Footer />
  </div>
</template>

<script>
  import Header from "../../components/header/Header";
  import Footer from "../../components/footer/Footer";
  import feather from "feather-icons";
  import { ValidationObserver } from "vee-validate";
  import { ValidationProvider } from "vee-validate/dist/vee-validate.full.esm";
  export default {
    components: {
      Header,
      Footer,
      ValidationObserver,
      ValidationProvider,
    },
    data() {
      return {
        formData: {
          name: "",
          email: "",
          subject: "",
          message: "",
        },
        items: [
          {
            thumb: require("../../assets/images/blog/bl-big-01.jpg"),
            src: "https://www.youtube.com/watch?v=ZOoVOfieAF8",
          },
        ],
        metaList: [
          {
            icon: "clock",
            text: "May 4, 2022",
          },
          {
            icon: "",
            text: "",
          },
          {
            icon: "message-circle",
            text: "",
          },
          {
            icon: "heart",
            text: "Like",
          },
        ],
        index: null,
      };
    },

    methods: {
      iconSvg(icon) {
        return feather.icons[icon].toSvg();
      },
      onSubmit() {
        console.log(this.formData);
      },
    },
  };
</script>
