<template>
<q-page class="">

    <q-page-container style="padding-top: 0;">
    <!-- Hero Section -->
      <div class="hero-container relative-position" style="height: 300px;">
        <q-img src="/images/travel-banner.jpg" class="absolute-full" style="z-index: -1; background-color: transparent;">
          <div class="absolute-center text-center text-white" style="background: transparent;">
            <div class="text-h2 text-weight-bold">Travel Centers</div>
          </div>
        </q-img>
      </div>

      <!-- Main Content -->
      <div class="q-pa-md">
        <!-- Find Travel Center Section -->
        <div class="bg-grey-2 q-pa-lg q-my-lg rounded-borders">
          <div class="row justify-center text-center">
            <div class="col-12">
              <p class="text-h5 q-mb-md">
                <span class="text-weight-bold">Your Home Away from Home</span> — Find an AMBEST Travel Center near you.
              </p>
              <q-btn color="primary" label="Locate a Travel Center" class="q-py-sm text-white" />
            </div>
          </div>
        </div>
        </div>
        <q-container class="q-mt-md q-rt-lg">
            <div class="row items-center q-gutter-xl">
            <!-- Text Section -->
            <div class="col-12 col-md-6">
                <h5 class="text-h5">
                A Network Built on <strong>Trust</strong> and <strong>Tradition</strong>
                </h5>
                <p class="q-mt-sm text-body1">
                Since 1988, AMBEST has been America’s Best Travel Centers—a member-owned network of
                independent truck stops and service centers. Unlike corporate-owned chains, AMBEST
                locations are family-run businesses where owners are hands-on, ready to provide personalized
                care and exceptional service. Here, you’re not just another traveler—you’re part of the family.
                </p>
                <div class="q-mt-md row wrap q-gutter-sm">
                <q-btn unelevated color="primary" label="Download Location List" class="q-px-md" />
                <q-btn outline color="primary" label="Print Location List" class="q-px-md" />
                </div>
            </div>

            <!-- Logo Section -->
            <div class="col-12 col-md-4 text-center">
                <q-img src="/images/ambest-logo3.png" contain style="max-width: 250px; height: auto;" />
            </div>
            </div>
  </q-container>






    </q-page-container>
  </q-page>
</template>

<script>
import { defineComponent, ref } from 'vue';

export default defineComponent({
  name: 'AmbestWebpage',
  setup() {
    const search = ref('');

    return {
      search
    };
  }
});
</script>

<style scoped>
.container {
  max-width: 1200px;
}

@media (max-width: 768px) {
  .text-section {
    text-align: center;
  }
  .btn-group {
    justify-content: center;
  }
}


</style>
