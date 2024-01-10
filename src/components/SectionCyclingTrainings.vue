<template>
    <section class="my_container text-center mx-auto mb-5">
        <div class="my_titles-sections">
            <h1>Our Professional Cycling Trainings</h1>
            <p>Learn from the mountain bike expert.</p>
        </div>
        <div class="d-flex w-100">
            <div v-for="card, index in  CyclingTrainings " class="trainings-card" v-show="cardToShow.includes(index)">
                <p class="fw-bold">{{ card.name }}</p>
                <img :src="`/src/assets/img/${card.img}`">
                <button type="button" class="btn btn-dark">View</button>
            </div>
        </div>
        <div class="w-100 text-center carousel_button mt-4">
            <button type="button" class="btn btn-light me-2"><i class="fa-solid fa-chevron-left"></i></button>
            <button type="button" class="btn btn-light ms-2"><i class="fa-solid fa-chevron-right"></i></button>
        </div>
    </section>
</template>
<script>
export default {
    props: {
        CyclingTrainings: Object,
    },
    data() {
        return {
            cardToShow: [0, 1, 2, 3]
        }
    },
    methods: {
        /* showNextCard(cardToShow) {
            numeromaggiore = this.cardToShow[this.cardToShow.length]
            this

        } */

    }

}
</script>
<style lang="scss" scoped>
section.my_container {


    div.trainings-card {
        width: calc((100% / 4) - 2.6rem);
        margin: 0 1.3rem;
        position: relative;
        overflow: hidden;
        background-color: white;
        border: 5px solid black;

        p {
            position: absolute;
            top: 15px;
            left: 20px;
            color: white;
            z-index: 4;

        }

        &:hover img {
            filter: brightness(1);
        }

        &:hover button {
            display: block;
        }

        img {
            width: 100%;
            filter: brightness(0.7);
        }


        button {
            position: absolute;
            z-index: 3;
            bottom: 20px;
            left: 20px;
            background-color: black;
            border-radius: 1px;
            font-weight: bold;
            font-size: 0.8rem;
            display: none;
        }


    }

    div.carousel_button {
        button {
            border: 1px solid black;
            border-radius: 1px;

            i {
                font-size: 0.8rem;
                padding: 0 0.2rem;
            }
        }
    }
}
</style>