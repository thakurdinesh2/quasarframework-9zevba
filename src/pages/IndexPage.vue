<template>
  <q-page class="column flex-center">
    <img
      alt="Quasar logo"
      src="~assets/homePage.png"
      style="width: 400px; height: 280px"
    />

    <div class="q-mt-xl">
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
    <q-page-container>
      <q-page class="q-pa-md">
        <p class="q-mt-md q-mr-sm">
          Ornare rhoncus nunc ut felis. Faucibus dolor at ultrices tincidunt.
          Pulvinar sed justo et viverra pellentesque. Mauris augue nulla proin
          vel a. Facilisis fringilla molestie dignissim elit orci malesuada.
          Lorem sit sagittis vitae nulla id. Mauris ipsum sed sed faucibus.
          Nulla amet metus gravida orci faucibus nisl eros arcu lorem. Nullam
          ornare molestie nam id gravida volutpat bibendum sem feugiat. Neque
          vulputate in et maecenas porta mi tellus. In massa porttitor urna quis
          volutpat at.
        </p>
      </q-page>
    </q-page-container>
  </q-page>
</template>

<script setup>
import { ref } from 'vue';

const count = ref(0);

const min = 1;
const max = 100;
</script>
