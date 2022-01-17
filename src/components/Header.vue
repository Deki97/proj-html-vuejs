<template>
    <header>
        <div class="my-container">
            <div class="header-wrapper">
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
    </header>
</template>


<script>
export default {
    name: 'Header'
}
</script>


<style lang="scss" scoped>
header {
    background-color: #21333e;
    color: #c0c3d0;
    font-weight: 300;

    .my-container {
        .header-wrapper {
            .header-top {
                display: flex;
                justify-content: space-between;
                font-size: 12px;
                padding: 10px 0;

                .timetables .icon {
                    margin-right: 5px;
                }

                .contacts {
                    display: flex;

                    & > div {
                        margin-right: 20px;
                    }

                    .telephone .icon,
                    .mail .icon {
                        margin-right: 5px;
                    }
                    
                    .social {
                        & > span {
                            margin-right: 25px;
                        }
                    }
                }
            }
        }
    }
}
</style>