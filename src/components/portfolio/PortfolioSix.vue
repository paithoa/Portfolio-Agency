<template>
  <div>
    <v-tabs v-model="tab" centered flat hide-slider color="primary">
      <v-tab :ripple="false" v-for="item in tabItems" :key="item.id">{{
        item.name
      }}</v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item
        v-for="item in tabContent"
        :key="item.id"
        class="portfolio-wrapper portfolio-list mt--60"
      >
        <v-row class="row--5" id="animated-thumbnials">
          <v-col
            lg="4"
            md="4"
            sm="6"
            cols="12"
            v-for="(item, i) in item.content"
            :key="i"
            @click="index = i"
          >
            <div class="portfolio_style--3">
              <div class="thumb">
                <a :href="`${item.routerLink}`" target="_blank"
                  ><img :src="item.src" alt="personal portfolio"
                /></a>
                <div class="port-hover-action">
                  <div class="content">
                    <h3>
                      <router-link to="/portfolio-details">{{
                        item.title
                      }}</router-link>
                    </h3>
                  </div>
                </div>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-tab-item>
    </v-tabs-items>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        tab: null,
        index: null,
        tabItems: [
          {
            id: 1,
            name: "All",
          },
        
        ],
        tabContent: [
          {
            id: 1,
            content: [
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-1.jpg"),
                title: `4D Medical`,
                routerLink:'https://4dmedical.com/'
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-2.jpg"),
                title: `The Good Guys`,
                 routerLink:'https://www.thegoodguys.com.au/'
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-3.jpg"),
                title: `RMIT`,
                 routerLink:'https://www.rmit.edu.au/'
              },
            ],
          },
          {
            id: 2,
            content: [
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-4.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-5.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-6.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-1.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-2.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-3.jpg"),
                title: `Mr. Joharuin Joly`,
              },
            ],
          },
          {
            id: 3,
            content: [
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-1.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-2.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-3.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-4.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-5.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-6.jpg"),
                title: `Mr. Joharuin Joly`,
              },
            ],
          },
          {
            id: 4,
            content: [
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-4.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-5.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-6.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-1.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-2.jpg"),
                title: `Mr. Joharuin Joly`,
              },
            ],
          },
          {
            id: 5,
            content: [
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-1.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-3.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-2.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-4.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-5.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-6.jpg"),
                title: `Mr. Joharuin Joly`,
              },
            ],
          },
          {
            id: 6,
            content: [
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-4.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-5.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-6.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-1.jpg"),
                title: `Mr. Joharuin Joly`,
              },
              {
                src: require("../../assets/img/project/portfolio-3/protfolio-2.jpg"),
                title: `Mr. Joharuin Joly`,
              },
            ],
          },
        ],
      };
    },
  };
</script>
