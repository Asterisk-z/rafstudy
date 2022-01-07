<template>
    <Head title="Log in" />

    <section>
        <div class="container-fluid">
            <div class="row">
                <div class="col-xl-7"><img class="bg-img-cover bg-center" src="assets/svg/book_lover.svg"
                        alt="looginpage"></div>

                <div class="col-xl-5 p-0">
                    <div class="login-card">
                        <form class="theme-form login-form" @submit.prevent="submit">
                            <h6 v-if="status" class="small text-success ">{{ status }}</h6>
                            <img src="assets/logo/logo.svg" alt="" srcset="" class="logo text-center mb-3 mt-3">
                            <!-- <h4 class="mb-3">Login</h4> -->
                            <div class="form-group">
                                <!-- <label>Email Address</label> -->
                                <div class="input-group"><span class="input-group-text"><i
                                            class="icon-email"></i></span>
                                    <input class="form-control"  id="email" type="email"  v-model="form.email" required autofocus placeholder="demo@gmail.com">
                                </div>
                            </div>
                            <div class="form-group">
                                <!-- <label>Password</label> -->
                                <div class="input-group"><span class="input-group-text"><i
                                            class="icon-lock"></i></span>
                                    <input class="form-control" type="password"  v-model="form.password" required autocomplete="current-password"
                                        placeholder="*********">
                                    <div class="show-hide"><span class="show"> <i
                                                class="fa fa-eye"></i> </span></div>
                                </div>
                            </div>
                            <div class="form-group">
                                <div class="checkbox">
                                    <jet-checkbox name="remember" v-model:checked="form.remember" />
                                    <label class="text-muted" for="checkbox1">Remember me</label>
                                </div>
                                <Link class="link" v-if="canResetPassword" :href="route('password.request')" >Forgot password?</Link>
                            </div>
                            <div class="form-group">
                                <button class="btn btn-primary btn-block" type="submit"  :class="{ 'opacity-25': form.processing }" :disabled="form.processing">Login</button>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

</template>

<script>
    import { defineComponent } from 'vue'
    import JetCheckbox from '@/Jetstream/Checkbox.vue'
    import { Head, Link } from '@inertiajs/inertia-vue3';

    export default defineComponent({
        components: {
            Head,
            JetCheckbox,
            Link,
        },

        props: {
            canResetPassword: Boolean,
            status: String
        },

        data() {
            return {
                form: this.$inertia.form({
                    email: '',
                    password: '',
                    remember: false
                })
            }
        },

        methods: {
            submit() {
                this.form
                    .transform(data => ({
                        ... data,
                        remember: this.form.remember ? 'on' : ''
                    }))
                    .post(this.route('login'), {
                        onFinish: () => this.form.reset('password'),
                    })
            }
        }
    })
</script>

<style>
 .logo {
            text-align: center;
            width: 100px;
            margin-left: 35%;
            margin-right: 50%;
        }

</style>
