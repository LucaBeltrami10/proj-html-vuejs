<template>
    <section class="my_container mx-auto mb-5">
        <div class="text-center">
            <h1 class="fw-bold fs-5">Special Packs</h1>
            <p>Select pricing plan to get more</p>
        </div>
        <div class="d-flex">
            <div v-for="plan in subscriptionPlan" class="my_card">
                <div class="upper_card text-center mb-2">
                    <img class="img-da-cambiare" :src="`/src/assets/img/${plan.img}`" alt="">
                    <h1 class="fs-6 fw-bold">{{ plan.plan }}</h1>
                    <p>{{ plan.description }}</p>
                </div>
                <div class="bottom_card text-center m-0">
                    <div v-for="service in plan.services"
                        class="d-flex justify-content-center align-items-center border-bottom mt-1 mx-4">
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
    div.my_card {
        width: calc((100% / 3) - 2rem);
        margin: 1rem;
        box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;

        p {
            font-size: 0.8rem;
        }

        i {
            font-size: 0.5rem;
        }

        div.upper_card {

            height: 200px;
            color: white;
            background-color: black;

            p {
                font-size: 0.7rem;
            }

        }

        div.bottom_card {
            background-color: white;
            color: gray;
            padding-top: 2rem;
            padding-bottom: 5rem;

            div {
                border-bottom: 1px solid lightgray;
            }
        }
    }

}
</style>