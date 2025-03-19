<template>
  <q-page class="">    <q-page-container style="padding: 0;">
    <!-- Hero Section -->
      <div class="hero-container relative-position" style="height: 300px;">
        <q-img src="/images/top-view-man-drinking-truck.png" class="absolute-full" style="z-index: -1; background-color: transparent;">
          <div class="absolute-center text-center text-white" style="background: transparent;">
            <div class="text-h2 text-weight-bold">AMBUCK$</div>
          </div>
        </q-img>
      </div>
      <div class="news-section row items-center bg-light q-ma-xl">
        <div class="col-12 col-md-6 text-center">
          <q-img
            src="/images/ambucks-logo-1.png"
            class="rounded-borders"
            fit="cover"
            style=" border-radius: 20px;"
            width="70%"
          />
        </div>
        <!-- right Side: Text Content -->
        <div class="col-12  col-md-6 q-px-xl">
          <div class="content q-pa-xl">
            <h5 class="text-h5"><span class="text-weight-bold">About AMBUCKS Rewards Program</span></h5>
            <p>AMBEST launched AMBUCKS, a professional driver loyalty
              program, in 1994. Professional drivers carn point(s) for every
              gallon purchased and can redeem these points at any
              AMBEST location nationwide. In addition to points, AMBUCK$
              cardholders earn one FREE shower credit for every 75+ diesel
              gallon purchase. Additional points can be earned through
              participating AMBEST Service Centers, 20 / 20 Bus Program
              Participants, and location specific offerings.</p>
              <p>
              Since the program's inception, our locations have issued billions
              of AMBUCK$ points and [XXX] showers to professional drivers.
              In addition, AMBEST has given away millions of points, cash and
              various other prizes through AMBUCK$ promotions. Subscribe
              here to sign up to receive our latest promotions.
              diesel
              </p>
              <q-btn label="Subscribe for AMBUCKS Rewards" rounded unelevated color="primary" class="q-mt-md text-bold" to="/about-ambest" />
          </div>
        </div>
      </div>


      <div class="q-ma-lg rounded-borders" style="">
        <div class="row justify-center text-center q-pa-lg" style="background-color: #f5f9fc !important;">
          <div class="col-12">
            <p class="text-h5 q-mb-md">
              <span class="text-weight-bold">Rewarding Every Gallon</span> — Earn Ambuck$ for Your Purchase at AMBEST Locations.
            </p>
            <q-btn color="primary" label="Locate a Travel Center" rounded class="q-py-sm text-white" />
          </div>
        </div>
      </div>

      <div class="news-section row items-center bg-light q-ma-xl">
        <div class="col-12 col-md-6 text-center">
          <q-img
            src="/images/Mask_group.png"
            class="rounded-borders"
            fit="cover"
            style=" border-radius: 20px;"
            width="70%"
          />
        </div>
        <!-- right Side: Text Content -->
        <div class="col-12  col-md-6 q-px-xl">
          <div class="content q-pa-xl">
            <h5 class="text-h5"><span class="text-weight-bold">How it Works</span></h5>
            <p>
                Register, swipe and start earning points, free showers <br>
                and prizes!
              </p>
              <q-btn label="Subscribe for AMBUCKS Rewards" rounded unelevated color="primary" class="q-mt-md text-bold" to="/about-ambest" />
          </div>
        </div>
      </div>

      <div class="custom-banner text-h3">
        <h5><span style="color: white;"><strong>Log In</strong> or <strong>Explore</strong> AMBEST Location Near You</span></h5>
        <div class="row justify-center" style="gap: 0.3rem;">
          <q-btn outline color="primary" style="background-color: white !important;" rounded unelevated class="q-mt-md text-bold" label="Check Your AMBUCK$ Balance" />
          <q-btn outline color="primary" style="background-color: white !important;" rounded unelevated class="q-mt-md text-bold" label="Locations Directory" />
        </div>
      </div>

      <div class="news-section row items-center bg-light">
        <!-- Left Side: Text Content -->
        <div class="col-12  col-md-6 q-px-xl">
          <div class="content q-pa-xl">
            <h5 class="text-h5 "><span class="text-weight-bold">This Month's AMBUCK$ <br>
              Promotions-</span>Don't Miss Out!</h5>
            <p>
              Check out current and previous promotions from AMBUCK$.
              Don't forget to download our app to find specific location
              offerings so you always get the best AMBUCK$ values.
            </p>
          </div>
        </div>
        <!-- Right Side: Image -->
        <div class="col-12 col-md-6 text-center">
          <q-img
            src="/images/Mask_group_30.png"
            class="rounded-borders"
            fit="cover"
            width="70%"
          />
        </div>
      </div>
    </q-page-container>
  </q-page>
</template>
<style>
.news-section {
  max-width: 80%;
  margin: auto;
  /* margin-left:10%; */
}
.custom-banner {
  background-color: #00659E; /* Light blue-gray background */
  padding: 10px 20px;
  border-radius: 20px; /* Rounded edges */
  text-align: center;
  font-size: 20px !important;
  font-weight: normal;
  color: #000; /* Black text */

  justify-content: center;
  align-items: center;
  max-width: 80%;
  margin: 1rem auto;
}
</style>
