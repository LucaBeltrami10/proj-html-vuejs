<template>
    <nav class="my_container container mx-auto py-1">
        <div class="row">
            <div class="col-3">
                <img id="gobike-logo" src="../assets/img/logo-gobike.png" alt="go bike logo">
            </div>
            <ul class="col-6 d-flex justify-content-center align-items-center mb-0">
                <li v-for="opt in headerNavEl" class="me-4 fw-semibold"><a href="">{{ opt.element }}</a></li>
            </ul>
            <div class="col-3 d-flex align-items-center">
                <i class="fa-solid fa-bars me-2 fs-4"></i>
                <button type="button" class="my_button btn btn-dark d-flex align-items-center ms-2">
                    <i class="fa-solid fa-helmet-un fs-3 me-2"></i>
                    <p class="m-0 fw-semibold">Upcoming Events</p>
                    <i class="fa-solid fa-arrow-right ms-1"></i>
                </button>
            </div>
        </div>
    </nav>
    <HeaderCarousel :SliderContent="SliderContent" />
</template>

<script>
import HeaderCarousel from './HeaderCarousel.vue';

export default {
    props: {
        headerNavEl: Array,
    },
    components: {
        HeaderCarousel,
    },
    data() {
        return {
            SliderContent: [
                {
                    img: 'slider-bike-9.jpg',
                    title: 'Professional Cycling Club',
                    paragraph: 'Learning cycling from the pros.'

                },
                {
                    img: 'slider-bike-4.jpg',
                    title: 'Professional Cycling Club',
                    paragraph: 'Learning cycling from the pros.'

                },
                {
                    img: 'slider-bike-12.jpg',
                    title: 'Professional Cycling Club',
                    paragraph: 'Learning cycling from the pros.'

                },
            ],

        }
    },
    methods: {

    },

}
</script>

<style lang="scss" scoped>
ul {
    li {
        font-size: 0.8rem;
    }
}

button.my_button {
    padding: 0.5rem 0.7rem 0.5rem 0.7rem;
    border-radius: 3px;

    p {
        font-size: 0.8rem;
    }

    i.fa-arrow-right {
        font-size: 0.7rem;
    }
}

#gobike-logo {
    width: 140px;
}
</style>