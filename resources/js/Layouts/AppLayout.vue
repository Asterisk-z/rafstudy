<template>
  <!-- <div>
    <Head :title="title" />

    <div class="min-h-screen bg-gray-100">
      <header class="bg-white shadow" v-if="$slots.header">
        <div class="max-w-7`xl mx-auto py-6 px-4 sm:px-6 lg:px-8">
          <slot name="header"></slot>
        </div>
      </header>
      <main>
        <slot></slot>
      </main>
    </div>
  </div> -->

  <!-- <div>

    <div class="min-h-screen bg-gray-100">
      <
      <header class="bg-white shadow" v-if="$slots.header">
        <div class="max-w-7`xl mx-auto py-6 px-4 sm:px-6 lg:px-8">
          <slot name="header"></slot>
        </div>
      </header>

    </div>


  </div> -->

  <div class="wrapper">
    <Head :title="title" />
    <!-- Sidebar  -->
    <div class="iq-sidebar">
      <div class="iq-sidebar-logo d-flex justify-content-between">
        <a href="#">
          <img src="images/logo/logo.svg" class="img-fluid" alt="" />
          <span>SMS</span>
        </a>
        <div class="iq-menu-bt-sidebar">
          <div class="iq-menu-bt align-self-center">
            <div class="wrapper-menu">
              <div class="main-circle">
                <i class="ri-arrow-left-s-line"></i>
              </div>
              <div class="hover-circle">
                <i class="ri-arrow-right-s-line"></i>
              </div>
            </div>
          </div>
        </div>
      </div>
      <Navigation />
    </div>
    <!-- TOP Nav Bar -->
    <div class="iq-top-navbar">
      <div class="iq-navbar-custom">
        <div class="iq-sidebar-logo">
          <div class="top-logo">
            <a href="#" class="logo">
              <img src="images/logo/logo.svg" class="img-fluid" alt="" />
              <span>SMS</span>
            </a>
          </div>
        </div>
        <nav class="navbar navbar-expand-lg navbar-light p-0">
          <div class="navbar-left">
            <div class="iq-search-bar">
              <form action="#" class="searchbox">
                <input
                  type="text"
                  class="text search-input"
                  placeholder="Type here to search..."
                />
                <a class="search-link" href="#"
                  ><i class="ri-search-line"></i
                ></a>
              </form>
            </div>
          </div>
          <button
            class="navbar-toggler"
            type="button"
            data-toggle="collapse"
            data-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent"
            aria-label="Toggle navigation"
          >
            <i class="ri-menu-3-line"></i>
          </button>
          <div class="iq-menu-bt align-self-center">
            <div class="wrapper-menu">
              <div class="main-circle">
                <i class="ri-arrow-left-s-line"></i>
              </div>
              <div class="hover-circle">
                <i class="ri-arrow-right-s-line"></i>
              </div>
            </div>
          </div>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ml-auto navbar-list">
              <li class="nav-item">
                <a href="#" class="search-toggle iq-waves-effect">
                  <div id="lottie-beil"></div>
                  <span class="bg-danger dots"></span>
                </a>
                <div class="iq-sub-dropdown">
                  <div class="iq-card shadow-none m-0">
                    <div class="iq-card-body p-0">
                      <div class="bg-primary p-3">
                        <h5 class="mb-0 text-white">
                          All Notifications<small
                            class="badge badge-light float-right pt-1"
                            >0</small
                          >
                        </h5>
                      </div>
                      <a href="#" class="iq-sub-card">
                        <div class="media align-items-center">
                          <div class="">
                            <img
                              class="avatar-40 rounded"
                              src="images/user/01.jpg"
                              alt=""
                            />
                          </div>
                          <div class="media-body ml-3">
                            <h6 class="mb-0">Emma Watson Nik</h6>
                            <small class="float-right font-size-12"
                              >Just Now</small
                            >
                            <p class="mb-0">95 MB</p>
                          </div>
                        </div>
                      </a>
                    </div>
                  </div>
                </div>
              </li>
              <li class="nav-item dropdown">
                <a href="#" class="search-toggle iq-waves-effect">
                  <div id="lottie-mail"></div>
                  <span class="bg-primary count-mail"></span>
                </a>
                <div class="iq-sub-dropdown">
                  <div class="iq-card shadow-none m-0">
                    <div class="iq-card-body p-0">
                      <div class="bg-primary p-3">
                        <h5 class="mb-0 text-white">
                          All Messages<small
                            class="badge badge-light float-right pt-1"
                            >0</small
                          >
                        </h5>
                      </div>
                      <a href="#" class="iq-sub-card">
                        <div class="media align-items-center">
                          <div class="">
                            <img
                              class="avatar-40 rounded"
                              src="images/user/01.jpg"
                              alt=""
                            />
                          </div>
                          <div class="media-body ml-3">
                            <h6 class="mb-0">Nik Emma Watson</h6>
                            <small class="float-left font-size-12"
                              >13 Jun</small
                            >
                          </div>
                        </div>
                      </a>
                    </div>
                  </div>
                </div>
              </li>
            </ul>
          </div>

          <ul class="navbar-list">
            <li>
              <a
                href="#"
                class="
                  search-toggle
                  iq-waves-effect
                  d-flex
                  align-items-center
                  bg-primary
                  rounded
                "
              >
                <img
                  src="images/user/1.jpg"
                  class="img-fluid rounded mr-3"
                  alt="user"
                />
                <div class="caption">
                  <h6 class="mb-0 line-height text-white">Odey Patrick</h6>
                  <span class="font-size-12 text-white">Available</span>
                </div>
              </a>
              <div class="iq-sub-dropdown iq-user-dropdown">
                <div class="iq-card shadow-none m-0">
                  <div class="iq-card-body p-0">
                    <div class="bg-primary p-3">
                      <h5 class="mb-0 text-white line-height">
                        Hello Odey Patrick
                      </h5>
                      <span class="text-white font-size-12">Available</span>
                    </div>
                    <a
                      href="profile.html"
                      class="iq-sub-card iq-bg-primary-hover"
                    >
                      <div class="media align-items-center">
                        <div class="rounded iq-card-icon iq-bg-primary">
                          <i class="ri-file-user-line"></i>
                        </div>
                        <div class="media-body ml-3">
                          <h6 class="mb-0">My Profile</h6>
                          <p class="mb-0 font-size-12">
                            View personal profile details.
                          </p>
                        </div>
                      </div>
                    </a>
                    <a
                      href="profile-edit.html"
                      class="iq-sub-card iq-bg-primary-hover"
                    >
                      <div class="media align-items-center">
                        <div class="rounded iq-card-icon iq-bg-primary">
                          <i class="ri-profile-line"></i>
                        </div>
                        <div class="media-body ml-3">
                          <h6 class="mb-0">Edit Profile</h6>
                          <p class="mb-0 font-size-12">
                            Modify your personal details.
                          </p>
                        </div>
                      </div>
                    </a>
                    <a
                      href="account-setting.html"
                      class="iq-sub-card iq-bg-primary-hover"
                    >
                      <div class="media align-items-center">
                        <div class="rounded iq-card-icon iq-bg-primary">
                          <i class="ri-account-box-line"></i>
                        </div>
                        <div class="media-body ml-3">
                          <h6 class="mb-0">Account settings</h6>
                          <p class="mb-0 font-size-12">
                            Manage your account parameters.
                          </p>
                        </div>
                      </div>
                    </a>
                    <a
                      href="privacy-setting.html"
                      class="iq-sub-card iq-bg-primary-hover"
                    >
                      <div class="media align-items-center">
                        <div class="rounded iq-card-icon iq-bg-primary">
                          <i class="ri-lock-line"></i>
                        </div>
                        <div class="media-body ml-3">
                          <h6 class="mb-0">Privacy Settings</h6>
                          <p class="mb-0 font-size-12">
                            Control your privacy parameters.
                          </p>
                        </div>
                      </div>
                    </a>
                    <div class="d-inline-block w-100 text-center p-3">
                      <a
                        class="bg-primary iq-sign-btn"
                        href="sign-in.html"
                        role="button"
                        >Sign out<i class="ri-login-box-line ml-2"></i
                      ></a>
                    </div>
                  </div>
                </div>
              </div>
            </li>
          </ul>
        </nav>
      </div>
    </div>
    <!-- TOP Nav Bar END -->
    <!-- Page Content  -->
    <div id="content-page" class="content-page">
      <div class="container-fluid">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import JetApplicationMark from "@/Jetstream/ApplicationMark.vue";
import JetBanner from "@/Jetstream/Banner.vue";
import JetDropdown from "@/Jetstream/Dropdown.vue";
import JetDropdownLink from "@/Jetstream/DropdownLink.vue";
import JetNavLink from "@/Jetstream/NavLink.vue";
import Navigation from "@/Jetstream/Navigation.vue";
import JetResponsiveNavLink from "@/Jetstream/ResponsiveNavLink.vue";
import { Head, Link } from "@inertiajs/inertia-vue3";

export default defineComponent({
  props: {
    title: String,
  },

  components: {
    Head,
    JetApplicationMark,
    JetBanner,
    JetDropdown,
    JetDropdownLink,
    JetNavLink,
    Navigation,
    JetResponsiveNavLink,
    Link,
  },

  data() {
    return {
      showingNavigationDropdown: false,
    };
  },

  methods: {
    switchToTeam(team) {
      this.$inertia.put(
        route("current-team.update"),
        {
          team_id: team.id,
        },
        {
          preserveState: false,
        }
      );
    },

    logout() {
      this.$inertia.post(route("logout"));
    },
  },
});
</script>
