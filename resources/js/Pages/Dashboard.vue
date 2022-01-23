<template>
  <app-layout title="Dashboard">
    <!-- <template #header>
      <h2 class="font-semibold text-xl text-gray-800 leading-tight">
        Dashboard
      </h2>
    </template> -->

    <div class="row">
      <div class="col-md-12">
        <h3 class="ml-3 mb-3 text-bold font-s-20">
          Patrick Odey (super admin)
        </h3>
      </div>
    </div>

    <div class="row">
      <div class="col-md-6 col-lg-3">
        <div
          class="iq-card iq-card-block iq-card-stretch iq-card-height bg-danger"
        >
          <div class="iq-card-body">
            <div class="text-center">
              <span class="font-s-17">Student</span>
            </div>
            <div class="text-center value-box">
              <span class="font-s-17 counter">102</span>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6 col-lg-3">
        <div
          class="iq-card iq-card-block iq-card-stretch iq-card-height bg-info"
        >
          <div class="iq-card-body">
            <div class="text-center">
              <span class="font-s-17">Teacher</span>
            </div>
            <div class="text-center value-box">
              <span class="font-s-17 counter">102</span>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6 col-lg-3">
        <div
          class="
            iq-card iq-card-block iq-card-stretch iq-card-height
            bg-success
          "
        >
          <div class="iq-card-body">
            <div class="text-center">
              <span class="font-s-17">Parent</span>
            </div>
            <div class="text-center value-box">
              <span class="font-s-17 counter">102</span>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6 col-lg-3">
        <div
          class="
            iq-card iq-card-block iq-card-stretch iq-card-height
            bg-primary
          "
        >
          <div class="iq-card-body">
            <div class="text-center">
              <span class="font-s-17">Class</span>
            </div>
            <div class="text-center value-box">
              <span class="font-s-17 counter">102</span>
            </div>
          </div>
        </div>
      </div>
      <div class="col-lg-6">
        <div class="iq-card iq-card-block iq-card-stretch iq-card-height">
          <div class="iq-card-body smaill-calender-home">
            <input type="text" class="flatpicker d-none" />
          </div>
        </div>
      </div>
    </div>
  </app-layout>
</template>

<script>
import { defineComponent } from "vue";
import AppLayout from "@/Layouts/AppLayout.vue";
import Welcome from "@/Jetstream/Welcome.vue";

export default defineComponent({
  components: {
    AppLayout,
    Welcome,
  },
});
</script>

<style>
</style>
