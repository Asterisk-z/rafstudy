<template>
  <Head title="Log in" />

  <section class="sign-in-page">
    <div class="container bg-white mt-5 p-0">
      <div class="row no-gutters">
        <div class="col-sm-6 align-self-center">
          <div class="sign-in-from">
            <a class="sign-in-logo mb-3 text-center" href="#"
              ><img
                src="images/logo/logo.svg"
                class="img-fluid m-auto"
                alt="logo"
            /></a>
            <h1 class="mb-0">Log in</h1>
            <p>Enter your credentials</p>
            <h6 v-if="status" class="small text-success">{{ status }}</h6>
            <form class="mt-4" @submit.prevent="submit">
              <div class="form-group">
                <label for="exampleInputEmail1">Email address</label>
                <input
                  type="email"
                  class="form-control mb-0"
                  id="exampleInputEmail1"
                  placeholder="Enter email"
                  v-model="form.email"
                  required
                  autofocus
                />
              </div>
              <div class="form-group">
                <label for="exampleInputPassword1">Password</label>
                <a
                  class="float-right"
                  v-if="canResetPassword"
                  :href="route('password.request')"
                  >Forgot password?</a
                >
                <input
                  type="password"
                  class="form-control mb-0"
                  id="exampleInputPassword1"
                  v-model="form.password"
                  required
                  autocomplete="current-password"
                  placeholder="*********"
                />
              </div>
              <div class="d-inline-block w-100">
                <div
                  class="
                    custom-control custom-checkbox
                    d-inline-block
                    mt-2
                    pt-1
                  "
                >
                  <jet-checkbox
                    name="remember"
                    v-model:checked="form.remember"
                  />
                  <label class="custom-control-label" for="customCheck1"
                    >Remember Me</label
                  >
                </div>
                <button
                  type="submit"
                  class="btn btn-primary float-right px-4"
                  :class="{ 'opacity-25': form.processing }"
                  :disabled="form.processing"
                >
                  Sign in
                </button>
              </div>
            </form>
          </div>
        </div>
        <div class="col-sm-6 text-center">
          <div class="sign-in-detail text-white">
            <div
              class="owl-carousel"
              data-autoplay="true"
              data-loop="true"
              data-nav="false"
              data-dots="true"
              data-items="1"
              data-items-laptop="1"
              data-items-tab="1"
              data-items-mobile="1"
              data-items-mobile-sm="1"
              data-margin="0"
            >
              <div class="item">
                <img
                  src="images/svg/book_lover.svg"
                  class="img-fluid mb-4"
                  alt="logo"
                />
              </div>
              <div class="item">
                <img
                  src="images/svg/book_lover.svg"
                  class="img-fluid mb-4"
                  alt="logo"
                />
              </div>
              <div class="item">
                <img
                  src="images/svg/book_lover.svg"
                  class="img-fluid mb-4"
                  alt="logo"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { defineComponent } from "vue";
import JetCheckbox from "@/Jetstream/Checkbox.vue";
import { Head, Link } from "@inertiajs/inertia-vue3";

export default defineComponent({
  components: {
    Head,
    JetCheckbox,
    Link,
  },

  props: {
    canResetPassword: Boolean,
    status: String,
  },

  data() {
    return {
      form: this.$inertia.form({
        email: "",
        password: "",
        remember: false,
      }),
    };
  },

  methods: {
    submit() {
      this.form
        .transform((data) => ({
          ...data,
          remember: this.form.remember ? "on" : "",
        }))
        .post(this.route("login"), {
          onFinish: () => this.form.reset("password"),
        });
    },
  },
});
</script>

<style>
</style>
