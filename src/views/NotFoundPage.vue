<template>
    <div class="container-fluid no-padding h-100">
        <div class="row justify-content-center align-items-center h-100">
            <!-- Begin Left Content -->
            <div class="col-xl-4 col-lg-4 no-padding d-flex justify-content-center">
                <!-- Begin Error -->
                <div class="error-02 mx-auto mb-3 text-center">
                    <h1 class="text-gradient-03">404</h1>
                    <h2>This page cannot be found! </h2>
                    <p>But we have lots of other pages for you to see. </p>
                    <router-link to="/">
                        <a href="#" class="btn btn-gradient-01">
                            Go Back
                        </a>
                    </router-link>
                </div>
                <!-- End Error -->
            </div>
            <!-- End Left Content -->
            <!-- Begin Right Content -->
            <div class="col-xl-8 col-lg-8 d-none d-sm-block no-padding">
                <div class="elisyam-bg bg-error-02" :style="setBackground()">
                </div>
            </div>
            <!-- End Right Content -->
        </div>
        <!-- End Row -->
    </div>
</template>
<script>
    import NotFoundPage from '../assets/07.jpg';

    export default {
        name: 'NotFoundPage',
        components: {
        },
        methods: {
            setBackground: function () {
                return "background: url(" + NotFoundPage + ") no-repeat center center";
            }
        }
    }
</script>
<style scoped>
</style>