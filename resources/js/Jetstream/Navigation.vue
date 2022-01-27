<template>
  <div id="sidebar-scrollbar">
    <nav class="iq-sidebar-menu">
      <ul id="iq-sidebar-toggle" class="iq-menu">
        <li class="iq-menu-title">
          <i class="ri-subtract-line"></i><span>Menu</span>
        </li>
        <li class="">
          <a href="#" class="iq-waves-effect"
            ><i class="ri-home-4-line"></i><span>Dashboard</span></a
          >
        </li>

        <li>
          <a
            href="#icons"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Admin</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="icons"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a :href="route('admin.main')"
                ><i class="ri-stack-line"></i>Main</a
              >
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#student"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Student Info</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="student"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a :href="route('admin.student.index')"
                ><i class="ri-stack-line"></i>Student category</a
              >
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Add Student</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Student List</a>
            </li>
            <li>
              <a href="#"
                ><i class="ri-facebook-fill"></i>Student Attendance Report</a
              >
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Student Group</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Disabled Student</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#academics"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Academics</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="academics"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Optional Subject</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Section</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Class</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Subjects</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Class Room</a>
            </li>
            <li>
              <a href="#"
                ><i class="ri-facebook-fill"></i>Assign Class Teacher</a
              >
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Class Routine</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Optional Subject</a>
            </li>
          </ul>
        </li>
      </ul>
    </nav>
    <div class="p-3"></div>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import { Link } from "@inertiajs/inertia-vue3";

export default defineComponent({
  components: {
    Link,
  },
  props: ["href", "active"],

  computed: {
    classes() {
      return this.active
        ? "inline-flex items-center px-1 pt-1 border-b-2 border-indigo-400 text-sm font-medium leading-5 text-gray-900 focus:outline-none focus:border-indigo-700 transition"
        : "inline-flex items-center px-1 pt-1 border-b-2 border-transparent text-sm font-medium leading-5 text-gray-500 hover:text-gray-700 hover:border-gray-300 focus:outline-none focus:text-gray-700 focus:border-gray-300 transition";
    },
  },
});
</script>
