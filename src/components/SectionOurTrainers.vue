<template>
    <section class="my_container mx-auto mb-5">
        <div class="my_titles-sections">
            <h1>Our Expert Trainers</h1>
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

                        <p class="fw-bold profession-tag">{{ card.profession }}</p>
                        <div class="d-flex social-icons justify-content-center">
                            <i class="fa-brands fa-facebook-f"></i>
                            <i class="fa-brands fa-square-instagram mx-2"></i>
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
<style lang="scss" scoped>
@use '../style/partials/variables' as *;

div.my_card {
    width: calc((100% / 4) - 2.4rem);
    margin: 0 1.2rem;
    position: relative;

    p {
        font-size: 0.9rem;
    }

    p.profession-tag {
        font-size: 0.7rem;
        color: $color-profession-tag;
    }

    div.img_container {
        height: 160px;
        overflow: hidden;
    }

    div.card-body {
        color: white;
        background-color: black;

        div.social-icons {

            i {
                color: white;
                font-size: 0.7rem;
            }
        }
    }

    img {
        object-fit: cover;
        object-position: center;
    }

    &:hover {
        img {
            filter: brightness(0.7);
            transform: scale(1.1);
        }
    }
}
</style>