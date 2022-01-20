<template>
    <!-- Services -->
    <div class="services">
        <div class="my-container">
            <div class="services-card-wrapper">
                <div class="single-service-card">
                    <div class="card-icon contrast-green-light">
                        <i class="fas fa-user-friends"></i>
                    </div>

                    <div class="card-title">
                        <h3>Human Capital</h3>
                    </div>

                    <div class="card-text paragraph">
                        <p>Humanizing business: Harness the power of technology to improve the way people work.</p>
                    </div>
                </div>

                <div class="single-service-card">
                    <div class="card-icon contrast-green-light">
                        <i class="fas fa-chart-pie"></i>
                    </div>

                    <div class="card-title">
                        <h3>Core Business</h3>
                    </div>

                    <div class="card-text paragraph">
                        <p>It takes innovative approaches to transform, modernize, and run existing platforms.</p>
                    </div>
                </div>

                <div class="single-service-card">
                    <div class="card-icon contrast-green-light">
                        <i class="fas fa-tachometer-alt"></i>
                    </div>

                    <div class="card-title">
                        <h3>Performance</h3>
                    </div>

                    <div class="card-text paragraph">
                        <p>Achieving maximum impact and value from investments in finance and supply chain.</p>
                    </div>
                </div>

                <div class="circles-grid">
                    <div class="circles-row">
                        <span v-for="item in 9" :key="item">
                            <i class="fas fa-circle"></i>
                        </span>
                    </div>
                    <div class="circles-row">
                        <span v-for="item in 9" :key="item">
                            <i class="fas fa-circle"></i>
                        </span>
                    </div>
                    <div class="circles-row">
                        <span v-for="item in 9" :key="item">
                            <i class="fas fa-circle"></i>
                        </span>
                    </div>
                    <div class="circles-row">
                        <span v-for="item in 9" :key="item">
                            <i class="fas fa-circle"></i>
                        </span>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- End Services -->
</template>


<script>
export default {
    name: 'Services'
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

.services {
    background-color: #eef4ed;
    padding: 100px 0 120px 0;
    position: relative;

    .services-card-wrapper {
        display: flex;

        .single-service-card {
            background-color: white;
            border-radius: 10px;
            margin: 0 10px;
            padding: 30px 30px;

            .card-icon {
                font-size: 24px;
                width: 50px;
                height: 50px;
                text-align: center;
                line-height: 50px;
                border-radius: 50%;
            }

            .card-title {
                h3 {
                    font-size: 20px;
                    margin-top: 20px;
                    margin-bottom: 15px;
                }
            }
        }

        .circles-grid {
            position: absolute;
            bottom: -29px;
            left: 50%;
            width: 135px;
            height: 58px;
            margin-left: -67.5px;
            color: $page-primary-color;
            font-size: 7px;
            z-index: 2;

            .circles-row {
                margin-top: 4px;
                span {
                    padding: 0 4px;
                    opacity: 0.3;
                }
            }
        }
    }
}
</style>