<template>
  <!-- Footer -->
  <div class="copyright">
    <!-- <v-container fluid> -->
      <!-- <v-row>
        <v-col lg="6" md="6" sm="6" cols="12">
          <div class="copyright-inner">
            <p>
              ©{{ new Date().getFullYear() }}
              <a href="http://www.nexthorizonaustralia.com/" target="_blank">Next Horizon Australia</a>. All Rights
              Reserved.
            </p>
          </div>
        </v-col>
        <v-col lg="6" md="6" sm="6" cols="12">
          <div class="text-center copyright-right text-md-right">
            <Social />
          </div>
        </v-col>
      </v-row> -->
    <!-- </v-container> -->
  </div>
  <!--// Footer -->
</template>

<script>
  // import Social from "../social/Social";
  export default {
    data() {
      return {};
    },
  };
</script>

<style lang="scss">
.copyright-inner {
  p {
    a {
      color: #222222;
      &:hover {
        color: #000;
      }
    }
  }
}
</style>
