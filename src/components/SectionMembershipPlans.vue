<template>
    <section class="my_container mx-auto mb-5">
        <div class="my_titles-sections">
            <div class="rounded overflow-hidden mb-2 mx-auto">
                <img class="" src="../assets/img/special-black-icon.png" alt="special photo">
            </div>
            <h1>Special Packs</h1>
            <p>Select pricing plan to get more</p>
        </div>
        <div class="d-flex">
            <div v-for="plan in subscriptionPlan" class="my_card">
                <div class="my_hover-card justify-content-center align-items-center">
                    <div class="text-center">
                        <h1 class="text-uppercase fw-bold fs-6">{{ plan.plan }}</h1>
                        <p class="fw-bold fs-5">${{ plan.price }}</p>
                        <button type="button" class="btn btn-light mt-5">Send Request!</button>
                    </div>
                </div>
                <div class="upper_card text-center mb-2">
                    <img class="img-da-cambiare" :src="`/src/assets/img/${plan.img}`" alt="">
                    <h1 class="fs-6 fw-bold">{{ plan.plan }}</h1>
                    <p>{{ plan.description }}</p>
                </div>
                <div class="bottom_card text-center m-0">
                    <div v-for="service, index in plan.services"
                        class="d-flex justify-content-center align-items-center mt-1 mx-4"
                        :class="index == (plan.services.length - 1) ? '' : 'border-bottom'">
                        <i :class="`fa-solid ${checkOrNot(service.included)} me-2 mb-1`"></i>
                        <p class=" pb-1  mb-1">
                            {{ service.service }}
                        </p>
                    </div>

                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    props: {
        subscriptionPlan: Object
    },
    data() {
        return {

        }
    },
    methods: {
        checkOrNot(toCheck) {
            if (toCheck === true) {
                return 'fa-check';
            } else {
                return 'fa-x';
            }

        }
    }


}
</script>
<style lang="scss" scoped>
section.my_container {
    div.my_titles-sections {
        div {
            height: 65px;
            width: 70px;

            img {
                width: 100%;
                height: 100%;
            }
        }
    }

    div.my_card {
        width: calc((100% / 3) - 2rem);
        margin: 1rem;
        position: relative;
        box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
        display: block;

        div.my_hover-card {
            height: 100%;
            width: 100%;
            background-color: black;
            display: none;
            position: absolute;
            color: white;

            button {
                background-color: rgba($color: #000000, $alpha: 0);
                color: white;
                font-size: 0.8rem;
                padding: 1rem 1.5rem;
                border-radius: 3px;
            }
        }

        &:hover div.my_hover-card {
            display: flex;
        }

        p {
            font-size: 0.8rem;
        }

        i {
            font-size: 0.5rem;
        }

        div.upper_card {

            height: 250px;
            color: white;
            background-image: url(../assets/img/trap2.png);
            background-position: start;
            background-repeat: no-repeat;
            background-size: 125%;

            p {
                font-size: 0.7rem;
            }

            img {
                margin-top: 1rem;
                width: 60px;
            }

        }

        div.bottom_card {
            background-color: white;
            color: gray;
            padding-top: 0;
            padding-bottom: 3.2rem;
        }
    }

}
</style>