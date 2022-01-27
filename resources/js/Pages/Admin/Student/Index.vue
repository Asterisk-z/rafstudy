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
      <div class="col-lg-6">
        <div class="iq-card iq-card-block iq-card-stretch iq-card-height">
          <h2>Admin Student Main</h2>
        </div>
      </div>
    </div>
  </app-layout>
</template>

<script>
import { defineComponent } from "vue";
import AppLayout from "@/Layouts/AppLayout.vue";

export default defineComponent({
  components: {
    AppLayout,
  },
});
</script>

<style>
</style>
