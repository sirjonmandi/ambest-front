<template>
  <q-page class="" style="">
    <q-page-container style="padding: 0 !important;">
    <!-- Hero Section -->
      <div class="hero-container relative-position" style="height: 300px;">
        <q-img src="/images/close-up-man-checking-mobile.png" class="absolute-full" style="z-index: -1; background-color: transparent;">
          <div class="absolute-center text-center text-white" style="background: transparent;">
            <div class="text-h2 text-weight-bold">Connect with Us!</div>
          </div>
        </q-img>
      </div>

      <div class="custom-banner text-h3">
        <h5><span style="color: white;">We're here to help — <strong>Reach out to the team with any inqiries.</strong></span></h5>
        <q-btn outline color="primary" style="background-color: white !important;" rounded  class="q-mt-md text-bold" label="SEND US A MESSAGE" />
      </div>
      <div class="text-center">
        <h5><span style="">Our<strong> Leadership</strong></span></h5>
      </div>
      <div class="row justify-center q-col-gutter-md">
        <div v-for="member in team" :key="member.name" class="col-3">
          <div class="text-center">
            <q-img :src="member.image" class="profile-image" style="height: 215px; width: 215px;" />
            <div class="">
              <div class="name">{{ member.name }}</div>
              <div class="position">{{ member.position }}</div>
            </div>
          </div>
        </div>
      </div>
        <!-- <div>contacts page</div> -->

        <div class="form-container" style="margin-top: 8rem;">
        <h2 class="">Have questions? <strong>Fill out the form and our team will get back to you within 24 hours.</strong></h2>

        <form action="#" method="POST">
            <div class="form-group row">
                <div class="form-field">
                    <label>First Name *</label>
                    <input type="text" required>
                </div>
                <div class="form-field">
                    <label>Last Name *</label>
                    <input type="text" required>
                </div>
            </div>

            <div class="form-group">
                <label>Phone *</label>
                <input type="tel" required>
            </div>

            <div class="form-group">
                <label>Email *</label>
                <input type="email" required>
            </div>

            <div class="form-group">
                <label>Which Services are You Looking For? *</label>
                <select required>
                    <option value="" disabled selected>Select One</option>
                    <option value="service1">Service 1</option>
                    <option value="service2">Service 2</option>
                    <option value="service3">Service 3</option>
                </select>
            </div>

            <div class="form-group">
                <label>Message *</label>
                <textarea required></textarea>
            </div>

            <q-btn label="SUBMIT" rounded unelevated color="primary" class="q-mt-md q-px-xl text-bold" to="/about-ambest" />
        </form>
    </div>

    <div class="faq-container" style="width: 80%; margin: auto;">
      <h5 class="text-h5"><span class="text-weight-bold">Answers to Your Frequently Asked Questions...</span></h5>
      <q-list class="faq-list">
        <q-expansion-item
          v-for="(item, index) in faqs"
          :key="index"
          expand-separator
          dense
          header-class="faq-item"
        >
          <template v-slot:header>
            <q-item-section>{{ item.question }}</q-item-section>
            <q-item-section side>
              <q-icon name="add" />
            </q-item-section>
          </template>
          <q-card>
            <q-card-section>
              {{ item.answer }}
            </q-card-section>
          </q-card>
        </q-expansion-item>
      </q-list>

      <div class="read-more text-center">
        <sapn class="text-weight-bold"  style="color: #00659E;">READ MORE</sapn>
      </div>
    </div>
    </q-page-container>
  </q-page>
</template>
<script setup>
import { ref } from "vue";
const team = ref([
{ image: "/images/Chuck.png", name: "Chuck Ryan", position: "President / CEO" },
        { image: "/images/tim.png", name: "Tim O'Brien", position: "Executive Vice President of Sales" },
        { image: "/images/Bob.png", name: "Bob Craig", position: "Director of Information Technology" },
        { image: "/images/Terri.png", name: "Terri Darroch", position: "Chief Financial Officer" },
        { image: "/images/Gabe.png", name: "Gabe Kelley", position: "Sr. Director — East Region" },
        { image: "/images/Sulser.png", name: "Joel Sulser", position: "Director of Service Centers" },
        { image: "/images/Shane.png", name: "Shane Vasel", position: "VP of Marketing & Purchasing" }
]);

const faqs = ref([
        { question: "How do I become an AMBEST Member?", answer: "You can become a member by signing up on our website." },
        { question: "What is AMBUCK$?", answer: "AMBUCK$ is our rewards program where you earn points on purchases." },
        { question: "How do I earn AMBUCK$ points?", answer: "You earn points when you make qualifying purchases." },
        { question: "Is there a fee to join AMBUCK$?", answer: "No, joining AMBUCK$ is completely free!" },
        { question: "Can I use my AMBUCK$ points at any location?", answer: "Points can be redeemed at participating locations." },
        { question: "I am not a truck stop owner. Can I still join AMBEST?", answer: "Yes, individuals can also join AMBEST." },
        { question: "Can I track my AMBEST points?", answer: "Yes, you can track your points through our website." },
        { question: "What is the AMBEST Fuel Card?", answer: "The AMBEST Fuel Card offers discounts on fuel purchases." },
        { question: "How do I use the AMBEST Fuel Card?", answer: "Simply swipe your card at participating fuel stations." },
        { question: "What are the benefits of using the AMBEST Fuel Card?", answer: "You can enjoy discounts, rewards, and more." }
    ]);
</script>

<style>
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
.profile-card{
  height:215px;
  width:215px;
}

.profile-card {
  /* max-width: 200px; */
  border-radius: 8px;
  text-align: center;
  /* box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1); */
}
.profile-image {
  border-radius: 8px;
}
.name {
  font-size: 16px;
  font-weight: bold;
  margin-top: 10px;
}
.position {
  font-size: 14px;
  color: #666;
}


.form-container {
  margin: auto;
    background: white;
    padding: 20px;
    width: 600px;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h2 {
    font-size: 18px;
    margin-bottom: 20px;
}

strong {
    font-weight: bold;
}

.form-group {
    margin-bottom: 15px;
}

.row {
    display: flex;
    gap: 10px;
}

.form-field {
    flex: 1;
}

label {
    font-size: 14px;
    display: block;
    margin-bottom: 5px;
    font-weight: bold;
}

input, select, textarea {
    width: 100%;
    padding: 8px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

textarea {
    height: 80px;
}

.checkbox {
    display: flex;
    align-items: center;
    gap: 5px;
}

button {
    background: #007bff;
    color: white;
    border: none;
    width: 100%;
    padding: 10px;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
}

button:hover {
    background: #0056b3;
}
</style>
