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
            ><i class="ri-list-check"></i><span>Admin Section</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="icons"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a :href="route('admin.main')"
                ><i class="ri-stack-line"></i>Admission</a
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
              <a href="#"><i class="ri-facebook-fill"></i>Student Attendance</a>
            </li>
            <li>
              <a href="#"
                ><i class="ri-facebook-fill"></i>Student Attendance Report</a
              >
            </li>
            <li>
              <a href="#"
                ><i class="ri-facebook-fill"></i>Subject Wise Attendance</a
              >
            </li>
            <li>
              <a href="#"
                ><i class="ri-facebook-fill"></i>Subject Wise Attendance
                Report</a
              >
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Student Group</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Student Promote</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Disabled Student</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Export Student</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Send SMS</a>
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
              <a href="#"><i class="ri-facebook-fill"></i>Assign Subject</a>
            </li>
            <li>
              <a href="#"><i class="ri-facebook-fill"></i>Class Routine</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#studymaterial"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Study Material</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="studymaterial"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Upload Content</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Assignment</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Syllabus</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Other Download</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#lessonplan"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Lesson Plan</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="lessonplan"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Lesson</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Topic</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Topic Overview</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Lesson Plan</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Lesson Plan Overview</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#fees"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Fees</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="fees"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Fees Group</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Fees Type</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Fees Invoice</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Bank Payment</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Fees Invoice Setting</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Fees Due</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#wallet"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Wallet</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="wallet"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Pending Deposit</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Approved Deposit</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Rejected Deposit</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Wallet Transaction</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Refund Request</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Wallet Report</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#bulkprint"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Bulk Print</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="bulkprint"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>ID Card</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Certificate</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Payroll Bulk Print</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#accounts"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Accounts</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="accounts"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Chart Of Account</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Bank Account</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Income</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Profit & Loss</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Expense</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Fund Transfer</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Reports</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#humanresource"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Human Resource</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="humanresource"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Designation</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Department</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Add Staff</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Staff Directory</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Staff Attendance</a>
            </li>
            <li>
              <a href="#"
                ><i class="ri-stack-line"></i>Staff Attendance Report</a
              >
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Payroll</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Payroll Report</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#leave"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Leave</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="leave"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Leave Type</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Leave Define</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Approve Leave Request</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Pending Leave Request</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#customfields"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Custom Fields</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="customfields"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Student Registration</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Staff Registration</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#chat"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Chat</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="chat"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Chat Box</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Invitation</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Blocked User</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Settings</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#examination"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Examination</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="examination"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Marks Grade</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Exam Type</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Exam Setup</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Exam Schedule</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Exam Attendance</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Mark Register</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Send Marks By SMS</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Setting</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#onlineexams"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Online Exams</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="onlineexams"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Question Group</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Question Bank</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Online Exams</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#homework"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Homework</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="homework"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Homework list</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Add Homework</a>
            </li>
            <li>
              <a href="#"
                ><i class="ri-stack-line"></i>Homework Evaluation Report</a
              >
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#communication"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Communicate</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="communication"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Notice Board</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Send Email</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Email/SMS log</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Event</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>SMS Template</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Email Template</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#library"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Library</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="library"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Book Categories</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Subject</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Add Book</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Book List</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Add Member</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Issue/Retrun Book</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>All Issued Book</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#inventory"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Inventory</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="inventory"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Item Category</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Item List</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Item Store</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Supplier</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Item Receive</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Item Receive List</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Item Sell</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Item Issue</a>
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#transport"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Transport</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="transport"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Route</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Vehicle</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Assign Vehicle</a>
            </li>
            <li>
              <a href="#"
                ><i class="ri-stack-line"></i>Student Transport Report</a
              >
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#dometry"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Dormitory</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="dometry"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Room Type</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Dormitory</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Dormitory Rooms</a>
            </li>
            <li>
              <a href="#"
                ><i class="ri-stack-line"></i>Student Dormitory Report</a
              >
            </li>
          </ul>
        </li>

        <li>
          <a
            href="#reports"
            class="iq-waves-effect collapsed"
            data-toggle="collapse"
            aria-expanded="false"
            ><i class="ri-list-check"></i><span>Reports</span
            ><i class="ri-arrow-right-s-line iq-arrow-right"></i
          ></a>
          <ul
            id="reports"
            class="iq-submenu collapse"
            data-parent="#iq-sidebar-toggle"
          >
            <li>
              <a href="#"><i class="ri-stack-line"></i>Student Report</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Guardian Report</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Student History</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Student Login Report</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Fee Statment</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Balance Fee Report</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Class Report</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Class Routine</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Exam Routine</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Merit List Report</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Online Exam Report</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Mark Sheet Report</a>
            </li>
            <li>
              <a href="#"
                ><i class="ri-stack-line"></i>Tabulation Sheet Report</a
              >
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Progress Card Report</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>User Log</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Previous Result</a>
            </li>
            <li>
              <a href="#"><i class="ri-stack-line"></i>Previous Record</a>
            </li>
          </ul>
        </li>

        <!-- <li>
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
          </ul>
        </li> -->
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
