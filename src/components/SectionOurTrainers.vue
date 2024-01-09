<template>
    <section class="my_container mx-auto mb-5">
        <div class="w-100 text-center">
            <h1 class="fw-bold fs-5">Our Expert Trainers</h1>
            <p>Learn to ride a bike from the expert</p>
        </div>
        <div class="w-100 d-flex">
            <div v-for="card in OurTrainers" class="my_card card">
                <div class="img_container">
                    <img :src="`/src/assets/img/${card.img}`" class="card-img-top" alt="...">
                </div>

                <div class="card-body text-center">
                    <div>
                        <p class="fw-bold mb-1">{{ card.name }} {{ card.surname }}</p>

                        <p class="fw-bold">{{ card.profession }}</p>
                        <div class="d-flex">
                            <i class="fa-brands fa-facebook-f"></i>
                            <i class="fa-brands fa-square-instagram"></i>
                            <i class="fa-brands fa-twitter"></i>
                        </div>
                    </div>

                </div>
            </div>
        </div>

    </section>
</template>
<script>
export default {
    props: {
        OurTrainers: Object
    }

}
</script>
<style lang="scss">
div.my_card {
    width: calc((100% / 4) - 2.4rem);
    margin: 0 1.2rem;

    p {
        font-size: 0.8rem;
    }

    div.img_container {
        height: 160px;
        overflow: hidden;
    }

    div.card-body {
        color: white;
        background-color: black;
    }
}
</style>