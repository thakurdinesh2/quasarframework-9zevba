<template>
  <div class="q-pa-md" style="text-align: center">
    <q-img
      src="~assets/home_page_img.png"
      style="max-width: 790px"
      class="q-pa-md"
    >
    </q-img>
  </div>
  <q-page class="column flex-center">
    <div>
      <span class="text-bold">Price $50</span>
      <span
        class="q-ml-sm"
        style="padding: 2px; border: 1px solid gray; border-radius: 15%"
      >
        -80%</span
      >
    </div>
    <div class="q-mt-md">
      <q-btn
        color="primary"
        dense
        round
        label="-"
        :disable="count === min"
        @click="count--"
      />
      <span class="q-mx-md text-bold">{{ count }}</span>

      <q-btn
        color="primary"
        dense
        round
        label="+"
        :disable="count === max"
        @click="count++"
      />
    </div>
    <q-page-container style="text-allign: center; max-width: 790px">
      <q-page class="q-pa-md">
        <strong
          >Ornare rhoncus nunc ut felis. Faucibus dolor at ultrices tincidunt.
          Pulvinar sed justo et viverra pellentesque.</strong
        >
        <p class="q-pt-md">
          Mauris augue nulla proin vel a. Facilisis fringilla molestie dignissim
          elit orci malesuada. Lorem sit sagittis vitae nulla id. Mauris ipsum
          sed sed faucibus. Nulla amet metus gravida orci faucibus nisl eros
          arcu lorem. Nullam ornare molestie nam id gravida volutpat bibendum
          sem feugiat. Neque vulputate in et maecenas porta mi tellus. In massa
          porttitor urna quis volutpat at.
        </p>

        <div class="row items-center" style="text-allign: center">
          <div class="col-6" style="padding: 5%; border: 1px solid gray">
            <span style="font-size: 0.7rem"
              >Guaranteed Safe & Secure Checkout</span
            >
          </div>
          <div class="col-1"></div>
          <div class="col-4" style="padding: 5%; border: 1px solid gray">
            <span style="font-size: 0.7rem">24/7</span><br />
            <span style="font-size: 0.7rem">Support</span>
          </div>
        </div>
      </q-page>
    </q-page-container>
  </q-page>
</template>
<script setup>
import { ref } from 'vue';
const count = ref(1);
const min = 1;
const max = 100;
slide: ref(1);
</script>
