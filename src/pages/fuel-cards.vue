<template>
  <q-page class="">
    <q-page-container style="padding-top: 0;">
    <!-- Hero Section -->
      <div class="hero-container relative-position" style="height: 300px;">
        <q-img src="/images/cards-banner.png" class="absolute-full" style="z-index: -1; background-color: transparent;">
          <div class="absolute-center text-center text-white" style="background: transparent;">
            <div class="text-h2 text-weight-bold">AMBEST Fuel Cards</div>
          </div>
        </q-img>
      </div>
      <div class="custom-banner text-h3">
        <h5><span style="color: white;">Fuel Savings, Simplified — <strong>Introducing AMBEST Fuel Cards</strong></span></h5>
        <q-btn outline color="primary" style="background-color: white !important;" rounded unelevated class="q-mt-md text-bold" label="EXPLORE TRAVEL CENTERS" />
      </div>

      <div class="news-section row items-center bg-light">
        <!-- Left Side: Text Content -->
        <div class="col-12  col-md-6 q-px-xl">
          <div class="content q-pa-xl">
            <h5 class="text-h5 ">About AMBEST <span class="text-weight-bold">Fuel Cards</span> Provide:</h5>
            <ul>
                <li>Exclusive fuel discounts for professional drivers and fleet operators</li>
                <li class="q-mt-sm">Flexible payment options to fit your needs</li>
                <li class="q-mt-sm">Expense tracking for better financial management</li>
                <li class="q-mt-sm">Accepted at over 1,000 AMBEST locations nationwide</li>
                <li class="q-mt-sm">Ideal for both fleet managers and solo drivers</li>
                <li class="q-mt-sm">Save money while keeping operations efficient and hassle-free</li>
                <li class="q-mt-sm">Access to AMBUCK$ points</li>
              </ul>
          </div>
        </div>
        <!-- Right Side: Image -->
        <div class="col-12 col-md-6 text-center">
          <q-img
            src="/images/card.png"
            class="rounded-borders"
            fit="cover"
            width="70%"
          />
        </div>
      </div>


      <div class="news-section row items-center bg-light">

        <div class="col-12 col-md-6 text-center">
          <q-img
            src="/images/fuel-refill.jpg"
            class="rounded-borders"
            fit="cover"
            style=" border-radius: 20px;"
            width="70%"
          />
        </div>
        <!-- right Side: Text Content -->
        <div class="col-12  col-md-6 q-px-xl">
          <div class="content q-pa-xl">
            <h5 class="text-h5 "><span class="text-weight-bold">Why</span> Choose AMBEST <span class="text-weight-bold">Fuel Cards</span> ?</h5>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aspernatur, inventore dicta culpa aliquid similique voluptatum repellat quis distinctio pariatur? Maiores, accusantium. Quasi id nobis dolore consequatur debitis eum, animi tempora.</p>
          </div>
        </div>
      </div>

      <div class="text-center">
        <h5 class="text-h5"><span class="text-weight-bold"> Find the Right AMBEST Fuel Card for You</span></h5>
        <p class="">AMBEST offers two fuel card options to fit the unique needs of drivers <br> and fleets. Compare below to see which one is the best fit for your business.</p>
        <p>Fuel Cards are accepted at all EFS-approved locations across the U.S. and Canada.</p>
      </div>

      <!-- <div class="q-mt-lg">
        <q-img src="path/to/credit-cards-image.png" class="q-mt-md" />
      </div> -->


      <div class="text-center">
        <h5 class="text-h5 "><span class="text-weight-bold">Exclusive</span>Offerings</h5>
      </div>
      <div class="news-section row items-center bg-light">
        <!-- Left Side: Text Content -->
        <div class="col-12  col-md-6 q-px-xl">
          <div class="content q-pa-xl">
            <h5 class="text-h5 "><span class="text-weight-bold">EFS UMA Crossroads </span>Fuel Card</h5>
            <p class="text-weight-bold">A Card Exclusively Designed for UMA Fleets</p>
            <p>The Crossroads fuel card offers significant fuel savings and nationwide acceptance.
                Enjoy an average discount of $0.35 to $0.45 per gallon at AMBEST Truck Stops.
                No monthly account fees.
                Convenience of purchasing gas or diesel anywhere EFS is accepted.
                A flat $1.50 transaction fee applies per purchase, making it a cost-effective solution for fleet fueling.
            </p>
          </div>
        </div>
        <!-- Right Side: Image -->
        <div class="col-12 col-md-6 text-center">
          <q-img
            src="/images/card.png"
            class="rounded-borders"
            fit="cover"
            width="70%"
          />
        </div>
      </div>
      <div class="text-center">
        <q-btn label="SEE ALL BENEFITS" rounded unelevated color="primary" class="q-mt-md text-bold" to="/about-ambest" />
      </div>
    </q-page-container>
  </q-page>
</template>
<style>
.custom-banner {
  background-color: #0057A3; /* Light blue-gray background */
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
.news-section {
  max-width: 80%;
  margin: auto;
  /* margin-left:10%; */
}
</style>
