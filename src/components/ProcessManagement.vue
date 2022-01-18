<template>
    <div class="process-management">
        <div class="mini-title">
            How It Works In Practice
        </div>

        <div class="heading-title">
            <span class="contrast-green-light">Process</span>
            Management
        </div>

        <div class="paragraph">
            We work with innovative methodologies to ensure that the entire reformatting process is done<br>
            from start to finish as planned.
        </div>

        <hr class="line-points">

        <div class="process-container">
            <div class="single-step">
                <div class="step-number contrast-green-light">
                    01
                </div>

                <div class="step-name">
                    <h3>Collection of information</h3>
                </div>

                <div class="paragraph">
                    Lorem ipsum dolor sit amet consectetur.
                </div>
            </div>

            <div class="single-step">
                <div class="step-number contrast-green-light">
                    02
                </div>

                <div class="step-name">
                    <h3>Strategic planning</h3>
                </div>

                <div class="paragraph">
                    Lorem ipsum dolor sit amet consectetur.
                </div>
            </div>

            <div class="single-step">
                <div class="step-number contrast-green-light">
                    03
                </div>

                <div class="step-name">
                    <h3>Assignment of responsibilities</h3>
                </div>

                <div class="paragraph">
                    Lorem ipsum dolor sit amet consectetur.
                </div>
            </div>

            <div class="single-step">
                <div class="step-number contrast-green-light">
                    04
                </div>

                <div class="step-name">
                    <h3>Formatting process</h3>
                </div>

                <div class="paragraph">
                    Lorem ipsum dolor sit amet consectetur.
                </div>
            </div>

            <div class="single-step">
                <div class="step-number contrast-green-light">
                    05
                </div>

                <div class="step-name">
                    <h3>Continuity formalization</h3>
                </div>

                <div class="paragraph">
                    Lorem ipsum dolor sit amet consectetur.
                </div>
            </div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'ProcessManagement'
}
</script>


<style lang="scss" scoped>
.process-management {
    text-align: center;
    padding: 120px 0;

    .line-points {
        height: 4px;
        color: #daeced;
        margin-top: 60px;
    }

    .process-container {
        display: flex;
        justify-content: space-between;

        .single-step {
            margin: 0 20px;
            position: relative;
            top: -40px;

            .step-number {
                display: inline-block;
                width: 40px;
                height: 40px;
                text-align: center;
                line-height: 40px;
                border-radius: 50%;
                font-weight: bold;
            }
            .step-name {
                h3 {
                    font-size: 20px;
                    margin-top: 20px;
                    margin-bottom: 15px;
                }
            }
        }
    }
}
</style>