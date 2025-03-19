<template>
  <q-page class="">
    <q-page-container style="padding: 0;">
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
          <div class="content">
            <h5 class="text-h5 ">About AMBEST <span class="text-weight-bold">Fuel Cards</span> Provide:</h5>
            <ul>
                <li>Exclusive fuel discounts for professional drivers and fleet operators</li>
                <li class="">Flexible payment options to fit your needs</li>
                <li class="">Expense tracking for better financial management</li>
                <li class="">Accepted at over 1,000 AMBEST locations nationwide</li>
                <li class="">Ideal for both fleet managers and solo drivers</li>
                <li class="">Save money while keeping operations efficient and hassle-free</li>
                <li class="">Access to AMBUCK$ points</li>
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


      <!-- <div class="row justify-center">
      <div class="col-12 col-md-5">
        <q-card class="my-card">
          <q-img src="efs-direct-card.png" class="card-image" />
          <q-card-section>
            <div class="text-h6 text-primary">EFS Direct Card</div>
            <p class="text-subtitle2">
              Ideal for businesses with multiple vehicles looking for customizable controls and detailed reporting.
            </p>
          </q-card-section>

          <q-list separator>
            <q-item v-for="(item, index) in directCardDetails" :key="index">
              <q-item-section>
                <q-item-label class="text-bold text-primary">{{ item.title }}</q-item-label>
                <q-item-label caption>{{ item.detail }}</q-item-label>
              </q-item-section>
            </q-item>
          </q-list>

          <q-card-actions align="center">
            <q-btn label="SEE ALL BENEFITS" class="btn-primary" />
            <q-btn label="VIEW ACCEPTING LOCATIONS" class="btn-secondary" />
          </q-card-actions>
        </q-card>
      </div>

      <div class="col-12 col-md-5">
        <q-card class="my-card">
          <q-img src="efs-preferred-card.png" class="card-image" />
          <q-card-section>
            <div class="text-h6 text-primary">EFS Preferred Card</div>
            <p class="text-subtitle2">
              Perfect for individual drivers or small fleets seeking straightforward savings, flexibility, and convenience.
            </p>
          </q-card-section>

          <q-list separator>
            <q-item v-for="(item, index) in preferredCardDetails" :key="index">
              <q-item-section>
                <q-item-label class="text-bold text-primary">{{ item.title }}</q-item-label>
                <q-item-label caption>{{ item.detail }}</q-item-label>
              </q-item-section>
            </q-item>
          </q-list>

          <q-card-actions align="center">
            <q-btn label="SEE ALL BENEFITS" class="btn-primary" />
            <q-btn label="VIEW ACCEPTING LOCATIONS" class="btn-secondary" />
          </q-card-actions>
        </q-card>
      </div>
    </div> -->

    <div class="row justify-center" >
      <table>
        <tbody>
          <tr>
            <td></td>
            <td><q-img src="/images/card.png" class="card-image" fit="cover"
              width="50%" height="100%"  />
          <q-card-section>
            <div class="text-h6 text-primary">EFS Preferred Card</div>
            <p class="text-subtitle2">
              Perfect for individual drivers or small fleets seeking straightforward savings, flexibility, and convenience.
            </p>
          </q-card-section></td>
            <td>
              <q-img src="/images/card.png" class="card-image" fit="cover"
              width="50%" height="100%" />
          <q-card-section>
            <div class="text-h6 text-primary">EFS Preferred Card</div>
            <p class="text-subtitle2">
              Perfect for individual drivers or small fleets seeking straightforward savings, flexibility, and convenience.
            </p>
          </q-card-section>
            </td>
          </tr>
        </tbody>
      </table>
    </div>


    <q-table
      flat
      bordered
      :rows="rows"
      :columns="columns"
      row-key="category"
      hide-bottom
    >
      <template v-slot:body-cell-category="props">
        <q-td :props="props">
          <strong class="text-primary">{{ props.row.category }}</strong>
        </q-td>
      </template>
    </q-table>


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
            src="/images/crossroads-card.png"
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
<script>
export default {
  data() {
    return {
      columns: [
        { name: "category", label: "", align: "left", field: "category" },
        { name: "businesses", label: "Businesses Managing Multiple Vehicles", align: "left", field: "businesses" },
        { name: "individuals", label: "Individual Drivers & Small Fleets", align: "left", field: "individuals" }
      ],
      rows: [
        { category: "Best For", businesses: "Businesses managing multiple vehicles", individuals: "Individual drivers and small fleets" },
        { category: "Discounts", businesses: "Aggressive discounts at AMBEST locations", individuals: "Competitive discounts at AMBEST locations & affiliates" },
        { category: "Fuel Controls", businesses: "Customizable spending limits and controls", individuals: "Simple, hassle-free purchasing" },
        { category: "Accepted At", businesses: "Nationwide fuel and maintenance locations", individuals: "AMBEST locations only" },
        { category: "Reporting", businesses: "Detailed Reports for tracking expenses", individuals: "AMBUCK$ Tiers: Direct and Preferred Memberships" }
      ]
    };
  }
};
</script>

<style scoped>
.my-card {
  padding: 20px;
  border-radius: 10px;
}

.card-image {
  height: 100px;
  object-fit: contain;
}

.btn-primary {
  background-color: #007bff;
  color: white;
  width: 100%;
  margin-top: 10px;
}

.btn-secondary {
  background-color: #0056b3;
  color: white;
  width: 100%;
  margin-top: 10px;
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
.news-section {
  max-width: 80%;
  margin: auto;
  /* margin-left:10%; */
}
</style>
