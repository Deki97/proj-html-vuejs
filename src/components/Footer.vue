<template>
    <footer>
        <!-- Footer Top Wrapper -->
        <div class="footer-top-wrapper">
            <div class="my-container">
                <div class="footer-top">
                    <div class="row">
                        <!-- Footer Col Left (Form) -->
                        <div class="col-8">
                            <div class="form">
                                <!-- Componente FooterForm -->
                                <FooterForm />
                            </div>
                        </div>
                        <!-- End Footer Col Left (Form) -->

                        <!-- Footer Col Right -->
                        <div class="col-4">
                            <div class="references">
                                <!-- Lista di menu / paragrafi che verrà poi presa tramite props da App.vue -->
                                <div class="title">
                                    <h3>Example Inc.</h3>
                                </div>

                                <div class="paragraph">
                                    <p v-for="(item, index) in objectText" :key="index">
                                        {{ item.text }}
                                    </p>
                                </div>

                                <!-- Contacts -->
                                <div class="references-list">
                                    <div class="single-reference">
                                        <div class="reference-icon">
                                            <i class="fas fa-phone-alt"></i>
                                        </div>
                                        
                                        <span class="reference-text">
                                            +1 (305) 1234-5678
                                        </span>
                                    </div>

                                    <div class="single-reference">
                                        <div class="reference-icon">
                                            <i class="fas fa-envelope"></i>
                                        </div>
                                        
                                        <span class="reference-text">
                                            hello@example.com
                                        </span>
                                    </div>

                                    <div class="single-reference">
                                        <div class="reference-icon">
                                            <i class="fas fa-map-marker-alt"></i>
                                        </div>
                                        
                                        <span class="reference-text">
                                            Main Avenue, 987
                                        </span>
                                    </div>
                                </div>
                                <!-- End Contacts -->

                                <div class="map-button">
                                    <button>
                                        View Map
                                    </button>
                                </div>
                            </div>
                        </div>
                        <!-- End Footer Col Right -->
                    </div>
                </div>
            </div>
        </div>
        <!-- End Footer Top Wrapper -->
        
        <!-- Footer Bottom Wrapper -->
        <div class="footer-bottom-wrapper">
            <div class="my-container">
                <div class="footer-bottom">
                    <!-- Footer Bottom Left -->
                    <div class="enjoy">
                        Enjoy the low price. We are tracking any intention of piracy.
                    </div>
                    <!-- End Footer Bottom Left -->

                    <!-- Footer Bottom Right -->
                    <div class="copyright">
                        &copy; 2020 NEXGEN is Proudly Powered by <span class="codings">Codings</span>.
                    </div>
                    <!-- End Footer  Bottom Right -->
                </div>
            </div>
        </div>
        <!-- End Footer Bottom Wrapper -->
    </footer>
</template>


<script>
import FooterForm from './FooterForm.vue';

export default {
    name: 'Footer',
    components: {
        FooterForm
    },
    props: {
        objectText: Object
    }
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

footer {
    .footer-top-wrapper {
        background-color: #111117;
        padding: 100px 0;

        .footer-top {
            .references {
                padding-left: 30px;

                .title {
                    h3 {
                        color: white;
                        font-size: 20px;
                        margin-bottom: 20px;
                    }
                }
                .single-reference {
                    display: flex;
                    align-items: center;
                    margin: 20px 0;

                    .reference-icon {
                        color: $page-primary-color;
                        background-color: #0e272d;
                        width: 35px;
                        height: 35px;
                        text-align: center;
                        line-height: 35px;
                        border-radius: 50%;
                    }

                    .reference-text {
                        color: $page-primary-color;
                        margin-left: 10px;
                        font-size: 14px;
                    }
                }

                .references-list {
                    margin-top: 30px;
                }

                .map-button {
                    button {
                        background-color: transparent;
                        color: white;
                        border: 1px solid $page-primary-color;
                        text-transform: uppercase;
                        font-size: 14px;
                        padding: 5px 20px;
                        border-radius: 3px;
                    }
                }
            }
        }
    }

    .footer-bottom-wrapper {
        background-color: black;
        color: #9a9ba2;
        border-bottom: 2px solid #9a9ba2;

        .footer-bottom {
            display: flex;
            justify-content: space-between;
            padding-top: 30px;
            padding-bottom: 5px;
            font-size: 14px;
            
            .copyright {
                .codings {
                    color: $page-primary-color;
                }
            }
        }
    }
}
</style>