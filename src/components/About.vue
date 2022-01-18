<template>
    <div class="about">
        <div class="row row-cols-2 g-0">
            <div class="col d-flex align-items-center">
                <div class="about-text">
                    <div class="mini-title">
                        About The Network
                    </div>

                    <div class="heading-title">
                        <span class="contrast-green">The</span>
                        Company
                    </div>

                    <div class="paragraph">
                        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras iaculis diam varius diam ultricies lacinia.</p>
                    </div>

                    <div class="number-stats">
                        <div class="single-stats">
                            <div class="number green">
                                0
                            </div>

                            <div class="target">
                                Employees
                            </div>

                            <div class="paragraph">
                                <p>Lorem ipsum dolor sit amet.</p>
                            </div>
                        </div>

                        <div class="single-stats">
                            <div class="number green">
                                0
                            </div>

                            <div class="target">
                                Partners
                            </div>

                            <div class="paragraph">
                                <p>Lorem ipsum dolor sit amet.</p>
                            </div>
                        </div>

                        <div class="single-stats">
                            <div class="number green">
                                0
                            </div>

                            <div class="target">
                                Customers
                            </div>

                            <div class="paragraph">
                                <p>Lorem ipsum dolor sit amet.</p>
                            </div>
                        </div>
                    </div>

                    <div class="buttons">
                        <PrimaryButton />

                        <!-- Come posso passare il text-color nero senza sovrascrivere il componente SecondaryButton? -->
                        <SecondaryButton />                    
                    </div>
                </div>
            </div>

            <div class="col">
                <div class="about-image"></div>
            </div>
        </div>
    </div>
</template>


<script>
import PrimaryButton from './PrimaryButton.vue';
import SecondaryButton from './SecondaryButton.vue';

export default {
    name: 'About',
    components: {
        PrimaryButton,
        SecondaryButton
    }
}
</script>


<style lang="scss" scoped>

.about {
    .about-text {
        margin-left: 320px;
        padding-right: 30px;

        .heading-title {
            span {
                padding: 0 10px;
                border-radius: 5px;
            }
        }

        .number-stats {
            display: flex;
            justify-content: space-between;
            margin-top: 40px;

            .single-stats {
                margin: 0 10px;

                .number {
                    font-size: 30px;
                    font-weight: 900;
                    padding-left: 15px;
                }

                .target {
                    font-size: 20px;
                    font-weight: 700;
                    margin-bottom: 10px;
                }
            }
        }

        .buttons {
            margin-top: 30px;
            padding-left: 10px;
        }
        
    }

    .about-image {
        background-image: url('../assets/img/about-5.jpg');
        height: 600px;
        background-size: cover;
        background-position: center;
    }
}
</style>