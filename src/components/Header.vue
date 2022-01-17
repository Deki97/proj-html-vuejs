<template>
    <header>
        <!-- Header Top Wrapper -->
        <div class="header-top-wrapper">
            <div class="my-container">
                <!-- Header Top -->
                <div class="header-top">
                    <!-- Header Top Left -->
                    <div class="timetables">
                        <span class="icon">
                            <i class="fas fa-clock"></i>
                        </span>

                        <span>
                            Open Hours: Mon - Sat - 9:00 - 18:00
                        </span>
                    </div>
                    <!-- End Header Top Left -->

                    <!-- Header Top Right -->
                    <div class="contacts">
                        <!-- Telephone -->
                        <div class="telephone">
                            <span class="icon">
                                <i class="fas fa-phone-alt"></i>
                            </span>

                            <span>
                                +1 (305) 1234-5678
                            </span>
                        </div>
                        <!-- End Telephone -->

                        <!-- Mail -->
                        <div class="mail">
                            <span class="icon">
                                <i class="fas fa-envelope"></i>
                            </span>

                            <span>
                                hello@example.com
                            </span>
                        </div>
                        <!-- End Mail -->

                        <!-- Social -->
                        <div class="social">
                            <span class="facebook icon">
                                <a href="#">
                                    <i class="fab fa-facebook-f"></i>
                                </a>
                            </span>

                            <span class="twitter icon">
                                <a href="#">
                                    <i class="fab fa-twitter"></i>
                                </a>
                            </span>

                            <span class="linkedin icon">
                                <a href="#">
                                    <i class="fab fa-linkedin-in"></i>
                                </a>
                            </span>
                        </div>
                        <!-- End Social -->
                    </div>
                    <!-- End Header Top Right -->
                </div>
                <!-- End Header Top -->
            </div>
        </div>
        <!-- End Header Top Wrapper -->


        <!-- Header Bottom Wrapper -->
        <div class="header-bottom-wrapper">
            <div class="my-container">
                <!-- Header Bottom -->
                <div class="header-bottom">
                    <nav>
                        <div class="nav-logo">
                            <span class="first-half">
                                Nex
                            </span>
                            <span class="second-half">
                                Gen
                            </span>
                        </div>

                        <div class="nav-menu">
                            <ul>
                                <li>
                                    <a href="#">Home</a>
                                </li>

                                <li>
                                    <a href="#">About</a>
                                </li>

                                <li>
                                    <a href="#">Projects</a>
                                </li>

                                <li>
                                    <a href="#" class="highlighted">Process</a>
                                </li>

                                <li>
                                    <a href="#">Testimonials</a>
                                </li>

                                <li>
                                    <a href="#">
                                        <i class="far fa-user"></i>
                                    </a>
                                </li>

                                <li>
                                    <a href="#"><PrimaryButton /></a>
                                </li>
                            </ul>
                        </div>
                    </nav>
                </div>
                <!-- End Header Bottom -->
            </div>
        </div>
        <!-- End Header Bottom Wrapper -->
    </header>
</template>


<script>
import PrimaryButton from './PrimaryButton.vue';

export default {
    name: 'Header',
    components: {
        PrimaryButton
    }
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

header {
    .header-top-wrapper {
        background-color: #21333e;

        .header-top {
            display: flex;
            justify-content: space-between;
            font-size: 12px;
            padding: 10px 0;
            color: #c0c3d0;
            font-weight: 300;

            .timetables .icon {
                margin-right: 5px;
            }

            .contacts {
                display: flex;

                .telephone {
                    margin-right: 20px;
                }

                .telephone .icon,
                .mail .icon {
                    margin-right: 5px;
                }
                
                .social {
                    & > span {
                        margin-left: 25px;
                    }
                }
            }
        }
    }

    .header-bottom-wrapper {
        background-image: url('../assets/img/bg-4.jpg');
        // test
        height: 680px;
        background-size: cover;
        background-repeat: no-repeat;

        .header-bottom {
            nav {
                display: flex;
                justify-content: space-between;
                align-items: center;
                padding: 15px 0;

                .nav-logo {
                letter-spacing: 2.5px;
                color: white;
                font-weight: 500;
                text-transform: uppercase;
            }

            .nav-menu {
                    ul {
                        display: flex;
                        align-items: center;

                        .highlighted {
                            color: $page-primary-color;
                        }

                        li {
                            text-transform: uppercase;
                            margin-left: 25px;

                            a {
                                font-size: 14px;
                                color: white;
                            }
                        }
                    }
                }
            }
        }
    }
}
</style>