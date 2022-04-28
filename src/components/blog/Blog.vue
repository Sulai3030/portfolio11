<template>
  <v-row>
    <!-- Start Blog Area  -->
    <v-col
      lg="4"
      md="4"
      sm="6"
      cols="12"
      v-for="(item, i) in blogContent"
      :key="i"
    >
      <div class="blog blog-style--1">
        <div class="thumbnail">
          <router-link to="/blog-details">
            <img class="w-100" :src="item.src" alt="Blog Images" />
          </router-link>
        </div>
        <div class="content">
          <p class="blogtype">{{ item.meta }}</p>
          <h4 class="heading-title">
            <router-link to="/blog-details">{{ item.title }}</router-link>
          </h4>
          <div class="blog-btn">
            <router-link to="/blog-details" class="rn-btn white--text">
              Read More
            </router-link>
          </div>
        </div>
      </div>
    </v-col>
    <!-- End Blog Area  -->
  </v-row>
</template>

<script>
  export default {
    data() {
      return {
        blogContent: [
          {
            src: require("../../assets/images/blog/52027722905_0df1f45afa_w.jpg"),
            meta: "Development",
            title: "First Post",
          },
          {
            src: require("../../assets/images/blog/51972410429_4508024bd4_w.jpg"),
            meta: "Development",
            title: "Getting tickets to the big show",
          },
          {
            src: require("../../assets/images/blog/51972192598_ac11da01ca_w.jpg"),
            meta: "Development",
            title: "Getting tickets to the big show",
          },
        ],
      };
    },
  };
</script>
