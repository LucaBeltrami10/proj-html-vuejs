<template>
    <div id="carouselExample" class="carousel slide">
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="../assets/img/slider-bike-9.jpg" class="d-block" alt="...">
                <div class="event-info">
                    <h1>Professional Cycling Club</h1>
                    <p>Learn cycling from the pros.</p>
                    <button class="btn btn-dark">Learn More <i class="fa-solid fa-arrow-right ms-1"></i></button>
                </div>
            </div>
            <div class="carousel-item">
                <img src="../assets/img/slider-bike-9.jpg" class="d-block" alt="...">
            </div>
            <div class="carousel-item">
                <img src="../assets/img/slider-bike-9.jpg" class="d-block" alt="...">
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
            <span class="carousel-control" aria-hidden="true"></span><!-- 
            <span class="visually-hidden">Next</span> -->
        </button>
    </div>
</template>

<script>
export default {

}
</script>
<style lang="scss">
#carouselExample {
    position: relative;
    width: 100%;
    height: 550px;
    overflow: hidden;

    div.carousel-inner {
        position: relative;

        div.carousel-item {
            img {
                width: 100%;
            }

            div.event-info {
                width: 220px;
                position: absolute;
                transform: translateY(-50%);
                top: 50%;
                left: 15%;
                color: white;

                h1 {
                    font-weight: 700;
                    font-size: 2.3rem;
                }

                p {
                    font-weight: 600;
                    font-size: 0.8rem;
                }

                button {
                    font-size: 0.8rem;
                    padding: 1rem 1.5rem 1rem 1.5rem;
                    border-radius: 3px;
                }
            }

        }
    }

    button.carousel-control-prev {
        height: 550px;
        position: absolute;
        left: 0;

    }
}
</style>