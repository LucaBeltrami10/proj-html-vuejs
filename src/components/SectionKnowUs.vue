<template>
    <section class="my_container mx-auto mb-5 overflow-hidden">
        <div class="row">
            <div class="my_left-col col-6 ms-auto px-3">
                <!-- <img class="my_img-rotate" src="../assets/img/bike-circle.png" alt="Bike player image"> -->
                <div class="my_main-img">
                    <img class="my_main-img" src="../assets/img/bike-player.png" alt="Bike player image">
                </div>

            </div>
            <div class="my_right-col col-5 ps-5">
                <h1 class="fw-bold fs-5">Do you want to be a professional cyclist?</h1>
                <p class="mb-0 pt-2">We offer 6 courses of varying difficulty and beatifoul scenary that cyclists of all
                    level
                    can enjoy. You
                    will learn cycling from professionls with our competent and experenced staff. You will have a lot of fun
                    with our amazing space.</p>
                <img class="mt-2 mb-4" src="../assets/img/divider.jpg" alt="Divider image">
                <div class="d-flex">
                    <i class="fa-solid fa-helmet-un fs-1 me-2"></i>
                    <div>
                        <h2 class="fs-6 fw-bold">Professional Team</h2>
                        <p>We make you professional by adding you sincerity as well as professionalism</p>
                    </div>
                </div>
                <div class="d-flex ">
                    <i class="fa-solid fa-helmet-un fs-1 me-2"></i>
                    <div>
                        <h2 class="fs-6 fw-bold">Professional Trainings</h2>
                        <p>We always ride with the best equipment, respecting nature and fun </p>
                    </div>
                </div>
                <button type="button" class="btn btn-dark d-flex align-items-center">
                    <p class="fw-bold m-0">Get to know us</p>
                    <i class="fa-solid fa-arrow-right ms-1"></i>
                </button>
            </div>
        </div>
    </section>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
@use '../src/style/general.scss' as *;

section.my_container {

    div.row {
        div.my_left-col {
            background-image: url(../assets/img/bike-circle.png);
            background-size: contain;
            background-repeat: no-repeat;
            background-position: center;
            position: relative;



            img.my_img-rotate {

                position: absolute;
            }

            div.my_main-img {
                z-index: 20;

                img.my_main-img {
                    z-index: 2;
                }
            }


            img {
                width: 100%;
            }
        }

        div.my_right-col {
            padding-top: 5rem;
            padding-right: 5rem;

            p {
                font-size: 0.65rem;
            }

            img {
                width: 80px;
            }

            button {
                padding: 1rem 1.5rem 1rem 1.5rem;
                border-radius: 3px;

                i {
                    font-size: 0.6rem;
                }
            }
        }
    }
}
</style>