<template>
    <section class="my_container mx-auto mb-5">
        <div class="text-center">
            <h1 class="fw-bold fs-5">Special Packs</h1>
            <p>Select pricing plan to get more</p>
        </div>
        <div class="d-flex">
            <div class="my_card">
                <div class="upper_card text-center mb-2">
                    <img class="img-da-cambiare" src="../assets/img/favicon-gobike.png" alt="">
                    <h1 class="fs-5 fw-bold">Basic</h1>
                    <p>Learn to ride a bike from...</p>
                </div>
                <div class="bottom_card text-center m-0">
                    <div>
                        <p class="border-bottom pb-1 mx-4 mb-1">
                            ciao
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
        /* checkOrNot(toCheck){
            if(toCheck === true){
                return <i class="fa-solid fa-check"></i>
            }else {
                return <i class="fa-solid fa-x"></i>
            }

        } */
    }


}
</script>
<style lang="scss" scoped>
section.my_container {
    div.my_card {
        width: calc((100% / 3) - 2rem);
        margin: 1rem;

        p {
            font-size: 0.8rem;
        }

        div.upper_card {

            height: 200px;
            color: white;
            background-color: black;

        }

        div.bottom_card {
            background-color: white;
        }
    }

}
</style>