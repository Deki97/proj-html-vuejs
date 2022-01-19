<template>
    <!-- Actions and Projects Section -->
    <div class="actions-and-projects">
        <div class="my-container">
            <!-- Actions and Projects Wrapper -->
            <div class="actions-and-projects-wrapper">
                <div class="mini-title">
                    We Do More For Everyone
                </div>

                <div class="heading-title">
                    Actions &#38; 
                    <span class="contrast-green-dark">
                        Projects
                    </span>
                </div>

                <div class="list-actions-projects">
                    <ul class="grey">
                        <li>
                            <a href="#" class="contrast-green-dark">All</a>
                        </li>

                        <li>
                            <a href="#">Institutional</a>
                        </li>

                        <li>
                            <a href="#">Social</a>
                        </li>

                        <li>
                            <a href="#">Events</a>
                        </li>

                        <li>
                            <a href="#">Innovation</a>
                        </li>

                        <li>
                            <a href="#">Environment</a>
                        </li>

                        <li>
                            <a href="#">Technology</a>
                        </li>
                    </ul>
                </div>

                <!-- First Row -->
                <div class="row row-cols-3">
                    <div class="col">
                        <div class="card-image">
                            <img src="../assets/img/project-1.jpg" alt="Card Image">
                            <div class="overlay"></div>
                        </div>

                        <div class="card-description">
                            Academic professional program in social media
                        </div>
                    </div>

                    <div class="col">
                        <div class="card-image">
                            <img src="../assets/img/project-2.jpg" alt="Card Image">
                            <div class="overlay"></div>
                        </div>

                        <div class="card-description">
                            President's speech at the annual meeting
                        </div>
                    </div>

                    <div class="col">
                        <div class="card-image">
                            <img src="../assets/img/project-3.jpg" alt="Card Image">
                            <div class="overlay"></div>
                        </div>

                        <div class="card-description">
                            International business trip in Shanghai
                        </div>
                    </div>
                </div>
                <!-- End First Row -->

                <!-- Second Row -->
                <div class="row row-cols-3">
                    <div class="col">
                        <div class="card-image">
                            <img src="../assets/img/project-4.jpg" alt="Card Image">
                            <div class="overlay"></div>
                        </div>

                        <div class="card-description">
                            Technology workshop with education theme
                        </div>
                    </div>

                    <div class="col">
                        <div class="card-image">
                            <img src="../assets/img/project-5.jpg" alt="Card Image">
                            <div class="overlay"></div>
                        </div>

                        <div class="card-description">
                            Donation of clothes and food to the partner NGO
                        </div>
                    </div>

                    <div class="col">
                        <div class="card-image">
                            <img src="../assets/img/project-6.jpg" alt="Card Image">
                            <div class="overlay"></div>
                        </div>

                        <div class="card-description">
                            Confraternization of the procurement team
                        </div>
                    </div>
                </div>
                <!-- End Second Row -->
            </div>
            <!-- End Actions and Projects Wrapper -->
        </div>
    </div>
    <!-- End Actions and Projects Section -->
</template>


<script>
export default {
    name: 'ActionsProjects'
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

.actions-and-projects {
    text-align: center;
    padding: 120px 0;
    background-color: #111117;

    .actions-and-projects-wrapper {
        .heading-title {
            color: white;
        }

        .list-actions-projects {
            ul {
                text-transform: uppercase;
                display: flex;
                justify-content: space-around;
                padding: 0 50px;
                margin: 30px 0;

                li {
                    a {
                        font-size: 14px;
                        font-weight: 500;
                        color: lightgrey;
                    }
                }

                .contrast-green-dark {
                    padding: 10px;
                }
            }
        }

        .row {
            margin-bottom: 25px;

            .col {
                position: relative;
                cursor: pointer;
                
                .card-image {
                    img {
                        border-radius: 10px;
                    }

                    // .overlay {
                    //     position: absolute;
                    //     top: 0;
                    //     left: 0;
                    //     width: 100%;
                    //     height: 100%;
                    //     background: rgba(0, 0, 0, .5);
                    //     overflow: hidden;
                    // }
                }

                .card-description {
                    position: absolute;
                    left: 0;
                    bottom: 30px;
                    color: white;
                    font-weight: bold;
                    padding: 0 20px;
                    font-size: 20px;
                }
            }
        }
    }
}
</style>