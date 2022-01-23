<template>
<div class="page-wrapper" id="pageWrapper">
        <!-- Page Header Start-->
        <div class="page-main-header">
            <div class="main-header-right row m-0">
                <div class="main-header-left">
                    <div class="logo-wrapper">
                        <a href="index.html">
                            <img class="img-fluid logo" src="assets/logo/logo.png" alt=""><span class="brand">SMS</span>
                        </a>
                    </div>
                    <div class="dark-logo-wrapper">
                        <a href="index.html">
                            <img class="img-fluid logo" src="assets/logo/logo.png" alt=""><span class="brand">SMS</span>
                        </a>
                    </div>
                    <div class="toggle-sidebar"><i class="status_toggle middle" data-feather="align-center"
                            id="sidebar-toggle"></i></div>
                </div>
                <div class="left-menu-header col">
                    <ul>
                        <li>
                            <form class="form-inline search-form">
                                <div class="search-bg"><i class="fa fa-search"></i>
                                    <input class="form-control-plaintext" placeholder="Search here.....">
                                </div>
                            </form><span class="d-sm-none mobile-search search-bg"><i class="fa fa-search"></i></span>
                        </li>
                    </ul>
                </div>
                <div class="nav-right col pull-right right-menu p-0">
                    <ul class="nav-menus">

                        <li>
                            <div class="mode"><i class="fa fa-moon-o"></i></div>
                        </li>
                        <li class="onhover-dropdown">
                            <div class="notification-box"><i data-feather="bell"></i><span class="dot-animated"></span>
                            </div>
                            <ul class="notification-dropdown onhover-show-div">
                                <li>
                                    <p class="f-w-700 mb-0">You have 3 Notifications<span
                                            class="pull-right badge badge-primary badge-pill">4</span></p>
                                </li>
                                <li class="noti-primary">
                                    <div class="media"><span class="notification-bg bg-light-primary"><i
                                                data-feather="activity"> </i></span>
                                        <div class="media-body">
                                            <p>Delivery processing </p><span>10 minutes ago</span>
                                        </div>
                                    </div>
                                </li>
                                <li class="noti-secondary">
                                    <div class="media"><span class="notification-bg bg-light-secondary"><i
                                                data-feather="check-circle"> </i></span>
                                        <div class="media-body">
                                            <p>Order Complete</p><span>1 hour ago</span>
                                        </div>
                                    </div>
                                </li>
                                <li class="noti-success">
                                    <div class="media"><span class="notification-bg bg-light-success"><i
                                                data-feather="file-text"> </i></span>
                                        <div class="media-body">
                                            <p>Tickets Generated</p><span>3 hour ago</span>
                                        </div>
                                    </div>
                                </li>
                                <li class="noti-danger">
                                    <div class="media"><span class="notification-bg bg-light-danger"><i
                                                data-feather="user-check"> </i></span>
                                        <div class="media-body">
                                            <p>Delivery Complete</p><span>6 hour ago</span>
                                        </div>
                                    </div>
                                </li>
                            </ul>
                        </li>
                        <li class="onhover-dropdown"><i data-feather="message-square"></i>
                        </li>
                        <li class="onhover-dropdown p-0">
                            <button class="btn btn-primary-light" type="button"><a href="login_two.html"><i
                                        data-feather="log-out"></i></a></button>
                        </li>
                    </ul>
                </div>
                <div class="d-lg-none mobile-toggle pull-right w-auto"><i data-feather="more-horizontal"></i></div>
            </div>
        </div>
        <!-- Page Header Ends                              -->
        <!-- Page Body Start-->
        <div class="page-body-wrapper horizontal-menu">
            <!-- Page Sidebar Start-->
            <header class="main-nav">
                <div class="sidebar-user text-center">


                    <img class="img-90 rounded-circle" src="assets/images/dashboard/1.png" alt="">
                    <a href="user-profile.html">
                        <h6 class="mt-3 f-14 f-w-600">Odey Patrick</h6>
                    </a>
                    <p class="mb-0 font-roboto">Super Admin</p>

                </div>
                <nav>
                    <div class="main-navbar">
                        <div class="left-arrow" id="left-arrow"><i data-feather="arrow-left"></i></div>
                        <div id="mainnav">
                            <ul class="nav-menu custom-scrollbar">
                                <li class="back-btn">
                                    <div class="mobile-back text-end"><span>Back</span><i class="fa fa-angle-right ps-2"
                                            aria-hidden="true"></i></div>
                                </li>
                                <li class="sidebar-main-title">
                                    <div>
                                        <h6>Menu </h6>
                                    </div>
                                </li>
                                <li class="dropdown"><a class="nav-link menu-title" href="javascript:void(0)"><i
                                            data-feather="home"></i><span>Dashboard</span></a>
                                    <ul class="nav-submenu menu-content">
                                        <li><a href="index.html">Default</a></li>
                                        <li><a href="dashboard-02.html">Ecommerce</a></li>
                                    </ul>
                                </li>
                                <li class="dropdown"><a class="nav-link menu-title" href="javascript:void(0)"><i
                                            data-feather="airplay"></i><span>Admin</span></a>
                                    <ul class="nav-submenu menu-content">
                                        <li><a href="general-widget.html">General</a></li>
                                        <li><a href="chart-widget.html">Chart</a></li>
                                    </ul>
                                </li>
                                <li class="dropdown"><a class="nav-link menu-title" href="javascript:void(0)"><i
                                            data-feather="layout"></i><span>Students</span></a>
                                    <ul class="nav-submenu menu-content">
                                        <li><a href="box-layout.html">Boxed</a></li>
                                        <li><a href="layout-rtl.html">RTL</a></li>
                                        <li><a href="layout-dark.html">Dark</a></li>
                                    </ul>
                                </li>
                                <li class="dropdown"><a class="nav-link menu-title" href="javascript:void(0)"><i
                                            data-feather="box"></i><span>
                                            Academics</span></a>
                                    <ul class="nav-submenu menu-content">
                                        <li><a href="state-color.html">State color</a></li>
                                        <li><a href="typography.html">Typography</a></li>
                                        <li><a href="avatars.html">Avatars</a></li>
                                    </ul>
                                </li>
                                <li class="dropdown"><a class="nav-link menu-title" href="javascript:void(0)"><i
                                            data-feather="box"></i><span>Fee Collections</span></a>
                                    <ul class="nav-submenu menu-content">
                                        <li><a href="state-color.html">State color</a></li>
                                        <li><a href="typography.html">Typography</a></li>
                                        <li><a href="avatars.html">Avatars</a></li>
                                        <li><a href="helper-classes.html">helper classes</a></li>
                                        <li><a href="grid.html">Grid</a></li>
                                    </ul>
                                </li>
                                <li class="dropdown"><a class="nav-link menu-title" href="javascript:void(0)"><i
                                            data-feather="folder-plus"></i><span>Dormitory</span></a>
                                    <ul class="nav-submenu menu-content">
                                        <li><a href="scrollable.html">Scrollable</a></li>
                                    </ul>
                                </li>
                            </ul>
                        </div>
                        <div class="right-arrow" id="right-arrow"><i data-feather="arrow-right"></i></div>
                    </div>
                </nav>
            </header>
            <!-- Page Sidebar Ends-->
            <div class="page-body">
                <div class="container-fluid">
                    <div class="page-header">
                        <div class="row">
                            <div class="col-sm-6">
                                <h3>Welcome Patrick(Super Admin)</h3>
                            </div>
                            <div class="col-sm-6">
                                
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Container-fluid starts-->
                <div class="container-fluid general-widget">
                    <div class="row">
                        <div class="col-sm-6 col-xl-3 col-lg-6">
                            <div class="card o-hidden border-0">
                                <div class="bg-info b-r-4 card-body">
                                    <div class="media static-top-widget">
                                        <div class="align-self-center text-center"><i data-feather="user"></i>
                                        </div>
                                        <div class="media-body"><span class="m-0">Students</span>
                                            <h4 class="mb-0 counter">0</h4><i class="icon-bg"
                                                data-feather="user-plus"></i>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-sm-6 col-xl-3 col-lg-6">
                            <div class="card o-hidden border-0">
                                <div class="bg-secondary b-r-4 card-body">
                                    <div class="media static-top-widget">
                                        <div class="align-self-center text-center"><i data-feather="user"></i>
                                        </div>
                                        <div class="media-body"><span class="m-0">Teachers</span>
                                            <h4 class="mb-0 counter">0</h4><i class="icon-bg"
                                                data-feather="user-plus"></i>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-sm-6 col-xl-3 col-lg-6">
                            <div class="card o-hidden border-0">
                                <div class="bg-primary b-r-4 card-body">
                                    <div class="media static-top-widget">
                                        <div class="align-self-center text-center"><i data-feather="user"></i>
                                        </div>
                                        <div class="media-body"><span class="m-0">Parents</span>
                                            <h4 class="mb-0 counter">0</h4><i class="icon-bg"
                                                data-feather="user-plus"></i>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-sm-6 col-xl-3 col-lg-6">
                            <div class="card o-hidden border-0">
                                <div class="bg-success b-r-4 card-body">
                                    <div class="media static-top-widget">
                                        <div class="align-self-center text-center"><i data-feather="user"></i>
                                        </div>
                                        <div class="media-body"><span class="m-0">Staffs</span>
                                            <h4 class="mb-0 counter">0</h4><i class="icon-bg"
                                                data-feather="user-plus"></i>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-6 xl-100 box-col-12">
                            <div class="card">
                                <div class="cal-date-widget card-body">
                                    <div class="row">
                                        <div class="col-xl-6 col-xs-12 col-md-6 col-sm-6">
                                            <div class="cal-datepicker">
                                                <div class="datepicker-here float-sm-end" data-language="en"> </div>
                                            </div>
                                        </div>
                                        <div class="col-xl-6 col-xs-12 col-md-6 col-sm-6">
                                           
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Container-fluid Ends-->
            </div>
            <!-- footer start-->
            <footer class="footer">
                <div class="container-fluid">
                    <div class="row">
                        <div class="col-md-6 footer-copyright">
                            <p class="mb-0">Copyright 2021-22 © All rights reserved.</p>
                        </div>
                        <div class="col-md-6">
                            <p class="pull-right mb-0">Made with <i
                                    class="fa fa-heart font-secondary"></i></p>
                        </div>
                    </div>
                </div>
            </footer>
        </div>
    </div>
</template>

<script>
    import { defineComponent } from 'vue'
    import AppLayout from '@/Layouts/AppLayout.vue'
    import Welcome from '@/Jetstream/Welcome.vue'

    export default defineComponent({
        components: {
            AppLayout,
            Welcome,
        },
    })
</script>

<style>


    .logo {
        max-width: 35px !important;
    }

    .brand {
        font-size: 20px;
        margin: 15px 0px 0px 10px;
        font-family: "poppins";
    }

    .page-main-header .main-header-right .nav-right .btn-primary-light {
        padding: 6px 10px;
        font-weight: 600;
    }

    .page-wrapper.compact-wrapper .page-body-wrapper header.main-nav .sidebar-user {
        margin-bottom: 0px;
    }

</style>
