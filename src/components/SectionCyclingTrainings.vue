<template>
    <section class="my_container text-center mx-auto mb-5">
        <div class="my_titles-sections">
            <h1>Our Professional Cycling Trainings</h1>
            <p>Learn from the mountain bike expert.</p>
        </div>
        <div class="container-fluid d-flex">
            <div v-for="card in  CyclingTrainings " class="trainings-card">
                <p class="fw-bold">{{ card.name }}</p>
                <img :src="`/src/assets/img/${card.img}`">
            </div>
        </div>
    </section>
</template>
<script>
export default {
    props: {
        CyclingTrainings: Object,
    }

}
</script>
<style lang="scss" scoped>
section {


    div.trainings-card {
        width: 180px;
        border: 4px solid black;
        position: relative;

        p {
            position: absolute;
            top: 20px;
            left: 20px;
            color: white;

        }

        img {
            width: 100%;
        }
    }
}
</style>