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
                            <div class="first-half">
                                Nex
                            </div>
                            <div class="second-half">
                                Gen
                            </div>
                        </div>

                        <div class="nav-menu">
                            <ul>
                                <!-- Tramite le props leggo i valori dei menu da App.vue accedendo all'oggetto -->
                                <li v-for="(item, index) in objectMenu" :key="index">
                                    <a href="#">{{ item.menu }}</a>
                                </li>

                                <li>
                                    <a href="#"><i class="far fa-user"></i></a>
                                </li>

                                <li>
                                    <a href="#"><PrimaryButton /></a>
                                </li>
                            </ul>
                        </div>
                    </nav>

                    <div class="banner-text col-6">
                        <div class="mini-title">
                            Human Resources
                        </div>

                        <div class="main-title">
                            <h1>Get More Productivity</h1>
                        </div>

                        <div class="paragraph">
                            <p>Planning, recruitment and selection process and performance evaluation of employees.</p>
                        </div>

                        <div class="buttons">
                            <PrimaryButton />
                            <SecondaryButton />
                        </div>

                        <div class="green-strip"></div>
                    </div>
                </div>
                <!-- End Header Bottom -->
            </div>
        </div>
        <!-- End Header Bottom Wrapper -->
    </header>
</template>


<script>
import PrimaryButton from './PrimaryButton.vue';
import SecondaryButton from './SecondaryButton.vue';

export default {
    name: 'Header',
    components: {
        PrimaryButton,
        SecondaryButton
    },
    props: {
        objectMenu: Object
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
            color: $page-secondary-color;
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
        background: linear-gradient(rgba(0,0,0,.4), rgba(0,0,0,.4)), url('../assets/img/bg-4.jpg');
        height: 680px;
        background-size: cover;
        background-repeat: no-repeat;

        .header-bottom {
            position: relative;

            nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;

            .nav-logo {
                display: flex;
                align-items: center;
                letter-spacing: 2.5px;
                color: white;
                font-weight: 500;
                text-transform: uppercase;

                .first-half {
                    color: #00a6a6;
                    background-color: #14322f;
                    padding: 5px 0 5px 20px;
                    border-top-left-radius: 20px;
                    border-bottom-left-radius: 20px;
                }

                .second-half {
                    padding-left: 2px;
                }
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

            .banner-text {
                position: absolute;
                transform: translateY(50%);
                
                .main-title {
                    h1 {
                        color: white;
                        font-weight: 900;
                        font-size: 50px;
                    }
                }

                .paragraph {
                    p {
                        color: $page-secondary-color;
                        font-size: 20px;
                        font-weight: 300;
                    }
                }

                .buttons {
                    margin-top: 40px;
                }

                .green-strip {
                    position: absolute;
                    background-color: $page-primary-color;
                    opacity: 0.5;
                    width: 280px;
                    height: 25px;
                    top: 110px;
                    left: 0;
                    z-index: -1;
                    border-radius: 3px;
                }
            }
        }
    }
}
</style>