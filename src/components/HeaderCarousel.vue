<template>
    <div id="carouselExampleAutoplaying" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div v-for="slide, index in SliderContent" class="carousel-item" :class="index === 0 ? 'active' : ''"
                data-bs-interval="5000">
                <img :src="`/src/assets/img/${slide.img}`" class="d-block" alt="Professional Cycling Photos">
                <div class="event-info">
                    <h1>{{ slide.title }}</h1>
                    <p>{{ slide.paragraph }}</p>
                    <button class="btn btn-dark">Learn More <i class="fa-solid fa-arrow-right ms-1"></i></button>
                </div>
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleAutoplaying"
            data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleAutoplaying"
            data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
    </div>
</template>

<script>
export default {
    props: {
        SliderContent: Object
    }


}
</script>
<style lang="scss">
#carouselExampleAutoplaying {
    position: relative;
    width: 100%;
    height: 550px;
    overflow: hidden;

    margin-bottom: 2.5rem;

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

        span.carousel-control-prev-icon {
            display: block;
            background-color: rgba($color: #000000, $alpha: 1.0);
        }


    }

    button.carousel-control-next {
        span.carousel-control-next-icon {
            display: block;
            background-color: rgba($color: #000000, $alpha: 1.0);
        }
    }

}
</style>