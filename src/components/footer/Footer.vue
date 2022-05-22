<template>
  <!-- Footer -->
  <footer class="-rn-footer" id="footer">
    <div class="rn-footer-wrapper footer">
      <v-container fluid>
        <v-row>
          <v-col lg="12">
            <div class="footer-top">
              <div class="content">
                <span>Starting a project!</span>
                <h4>Contact Us</h4>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
      <div class="footer-wrapper ptb--100">
        <v-container fluid>
          <v-row>
            <!-- Start Single Wedget -->
            <!-- <v-col lg="3" md="3" sm="6" cols="12">
              <div class="footer-widget">
                <h3 class="ft-title">Present Address</h3>
                <div class="content">
                  <p>
                    500 South Main Street <br />
                    Bishop, CA 93514
                  </p>
                </div>
              </div>
            </v-col> -->
            <!-- <v-col lg="3" md="3" sm="6" cols="12">
              <div class="footer-widget">
                <h3 class="ft-title">Home Address</h3>
                <div class="content">
                  <p>400 South Main Street <br />Bishop, CA 93514</p>
                </div>
              </div>
            </v-col> -->
            <v-col lg="6" md="6" sm="12" cols="12">
              <div class="footer-widget">
                <h3 class="ft-title">Email</h3>
                <div class="content">
                  <div class="address">
                    <p>
                      <a href="mailto:danielramezani@nexthorizonaustralia.com"
                        >danielramezani@nexthorizonaustralia.com</a
                      >
                    </p>
                    <p>
                      <a href="mailto:	handyhasan@nexthorizonaustralia.com"> handyhasan@nexthorizonaustralia.com</a>
                    </p>
                    <!-- <p><a href="tel:0123344556677">+012 3344 556677</a></p> -->
                  </div>
                </div>
              </div>
            </v-col>
            <v-col lg="6" md="6" sm="12" cols="12">
              <div class="footer-widget">
                <h3 class="ft-title">LinkedIn</h3>
                <div class="content">
                  <ul class="quick-link">
                    <li v-for="(link, i) in linkedIn" :key="i">
                      <a :href="link.RouteName">{{ link.name }}</a>
                      <!-- <router-link :to="link.RouteName">{{ link.name }}</router-link> -->
                    </li>
                  </ul>
                </div>
              </div>
            </v-col>
          </v-row>
        </v-container>
      </div>
    </div>

    <FooterTwo />
  </footer>
  <!--// Footer -->
</template>

<script>
import FooterTwo from './FooterTwo';
export default {
  components: {
    FooterTwo,
  },
  data() {
    return {
      linkedIn: [
        {
          name: 'Daniel Ramezani',
          RouteName: 'https://www.linkedin.com/in/daniel-r-a38a1359/',
        },
        {
          name: 'Handy Hassan',
          RouteName: 'https://www.linkedin.com/in/handy-hasan-a6aa73176/',
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
