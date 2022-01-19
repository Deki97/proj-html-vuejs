<template>
    <div class="feedback">
        <div class="my-container">
            <div class="feedback-wrapper">
                <div class="mini-title">
                    Customer Testimonials
                </div>

                <div class="heading-title">
                    Trusted
                    <span class="contrast-green-light">Feedback</span>
                </div>

                <div class="paragraph">
                    <p>We work intensively in search of ideals that can add up in the lives of our customers. This is what<br>
                    moves us and we are grateful for the recognition.</p>
                </div>

                <div class="feedback-cards">
                    <div class="single-feedback">
                        <div class="feedback-customer">
                            <img src="../assets/img/logo-1.png" alt="Logo Customer">
                        </div>

                        <div class="paragraph square">
                            <p>Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan orci rhoncus at pellentesque.</p>
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                        </div>

                        <div class="quote">
                            <i class="fas fa-quote-right"></i>
                        </div>
                    </div>

                    <div class="single-feedback">
                        <div class="feedback-customer">
                            <img src="../assets/img/logo-2.png" alt="Logo Customer">
                        </div>

                        <div class="paragraph square">
                            <p>Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan orci rhoncus at pellentesque.</p>
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                        </div>

                        <div class="quote">
                            <i class="fas fa-quote-right"></i>
                        </div>
                    </div>

                    <div class="single-feedback">
                        <div class="feedback-customer pingdom">
                            <img src="../assets/img/logo-3.png" alt="Logo Customer">
                        </div>

                        <div class="paragraph square">
                            <p>Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan orci rhoncus at pellentesque.</p>
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                        </div>

                        <div class="quote">
                            <i class="fas fa-quote-right"></i>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'Feedback'
}
</script>


<style lang="scss" scoped>
.feedback {
    background-color: #eef4ed;
    padding: 100px 0;

    .feedback-wrapper {
        .mini-title,
        .heading-title,
        .paragraph {
            text-align: center;
        }

        .feedback-cards {
            display: flex;
            margin-top: 40px;

            .single-feedback {
                background-color: white;
                border-radius: 10px;
                margin: 0 10px;
                padding: 30px 30px 10px 30px;
                position: relative;

                .feedback-customer {
                    width: 100px;
                    margin-bottom: 20px;

                    &.pingdom {
                        width: 80px;
                    }
                }

                .paragraph.square {
                    text-align: left;
                }

                .quote {
                    font-size: 20px;
                    color: lightgrey;
                    position: absolute;
                    bottom: 15px;
                    right: 25px;
                }
            }
        }
    }
}
</style>