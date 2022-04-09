<template>
  <v-col lg="12">
    <div class="tab-default">
      <v-tabs v-model="tab" flat hide-slider>
        <v-tab v-for="item in items" :key="item.id" :ripple="false">
          {{ item.name }}
        </v-tab>
      </v-tabs>

      <v-tabs-items v-model="tab">
        <v-tab-item
          transition="fade-transition"
          v-for="item in tabContent"
          :key="item.id"
        >
          <v-card flat>
            <v-card-text>
              <div class="single-tab-content">
                <ul>
                  <li v-for="(item, i) in item.content" :key="i">
                    <router-link to="/service"
                      >{{ item.title }}
                      <span> - {{ item.name }}</span></router-link
                    >
                    {{ item.desc }}
                  </li>
                </ul>
              </div>
            </v-card-text>
          </v-card>
        </v-tab-item>
      </v-tabs-items>
    </div>
  </v-col>
</template>
<script>
  export default {
    data() {
      return {
        tab: null,
        items: [
          {
            id: 1,
            name: "Main Skills",
          },
          {
            id: 2,
            name: "Work Experience",
          },
          {
            id: 4,
            name: "Technical Skills",
          },{
            id: 3,
            name: "Education",
          },
        ],

        tabContent: [
          {
            id: 1,
            content: [
              {
                title: "FrontEnd Developer",
                name: "FrontEnd Design",
                desc: "Use JavaScript, CSS, and HTML to create inviting website designs",
              },
              {
                title: "Web and user interface design and creation",
                name: "Development",
                desc: "Websites, Web experiences, ...",
              },
              {
                title: "",
                name: "",
                desc: "",
              },
            ],
          },
          {
            id: 2,
            content: [
              {
                title: "Frontend Engineer",
                name: "Freelance",
                desc: "2018 - Present",
              },
              {
                title: "Webmaster",
                name: "Mayapple Center for the Arts and Humanities | http://www.mayapplecenter.org/",
                desc: "2019 - Present",
              },
              {
                title: "Technical Writer/ Content Management Writer/Editor, Independent  Contractor",
                name: "Regeneron, Inc. | https://www.regeneron.com/",
                desc: "2017",
              },
              {
                title: "Technical Writer,  Independent Contractor",
                name: "New York City Dept. of Buildings | (http://www1.nyc.gov/site/buildings/index.page)",
                desc: "2017",
              },
              {
                title: "Technical Writer,  Independent  Contractor",
                name: "Maximus | https://nymedicaidchoice.com/",
                desc: "2016",
              },
            ],
          },
           {
            id: 4,
            content: [
              {
                title: "Languages:",
                name: "JavaScript, Python, CSS, HTML5",
                desc: "",
              },
              {
                title: "Libraries",
                name: "VueJs, React.js, React Native, Express, Node JS, jQuery, AJAX, Bootstrap",
                desc: "",
              },
              {
                title: "Databases:",
                name: "MongoDB, MySQL, NoSQL, Firebase",
                desc: "",
              },
              {
                title: "Templates:",
                name: "Handlebars",
                desc: "",
              },
              {
                title: "Version Control",
                name: "Jest/Enzyme",
                desc: "",
              },
              {
                title: "Testing:",
                name: "Git/GitHub",
                desc: "2016",
              },
               {
                title: "Platforms:",
                name: "Drupal, WordPress",
                desc: "",
              },
               {
                title: "Collaboration Software:",
                name: "Slack, Salesforce",
                desc: "",
              },
              {
                title: "Creative Cloud:",
                name: "Photoshop, Illustrator, Lightroom",
                desc: "",
              },
              {
                title: "Image Editors",
                name: "GIMP, Photoshop",
                desc: "",
              },
              {
                title: "Amazon Web Services (AWS)",
                name: "",
                desc: "",
              },
            ],
          },
          {
            id: 4,
            content: [
              {
                title: "Certificate, Full Stack Web Development: Columbia University",
                name: "Columbia University, New York City, NY",
                desc: "2017",
              },
              {
                title: "Master's in Fine Arts",
                name: "The New School University",
                desc: "2009",
              },
              {
                title: "Certificate in Publishing",
                name: "Emerson College, Boston, MA",
                desc: "2003",
              },
              {
                title: "Bachelor of Arts",
                name: "Emory University, Atlanta,GA",
                desc: "2001",
              },
              
            ],
          },
        ],
      };
    },
  };
</script>
