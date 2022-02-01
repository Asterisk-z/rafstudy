<template>
  <app-layout title="Dashboard">
    <div class="row">
      <div class="col-md-12">
        <h3 class="ml-3 mb-3 text-bold font-s-20">
          Patrick Odey (super admin)
        </h3>
      </div>
    </div>

    <h1 class="mx-3 my-3">Category</h1>
    <div class="row">
      <div class="col-md-12">
        <div class="row">
          <div class="col-sm-12">
          </div>
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
