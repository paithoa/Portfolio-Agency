<template>
  <!-- Footer -->
  <footer class="-rn-footer" id="footer">
    <div class="rn-footer-wrapper footer">
      <v-container fluid>
        <v-row>
          <v-col lg="12">
            <div class="footer-top">
              <div class="content">
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
      
            <v-col lg="3" md="3" sm="6" cols="12">
              <div class="footer-widget">
                <h3 class="ft-title">Address</h3>
                <div class="content">
                  <p>39 Mavho Street Bentleigh 3204,VIC</p>
                </div>
              </div>
            </v-col> 
            <v-col lg="6" md="6" sm="12" cols="12">
              <div class="footer-widget">
                <h3 class="ft-title">Email</h3>
                <div class="content">
                  <div class="address">
                    <p>
                      <a href="mailto:danielramezani@nexthorizonaustralia.com@domain.com">danielramezani@nexthorizonaustralia.com</a>
                    </p>
                    <p><a href="tel:+61414703015">+61414703015</a></p>
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

    <!-- <FooterTwo /> -->
  </footer>
  <!--// Footer -->
</template>

<script>

export default {
 
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
