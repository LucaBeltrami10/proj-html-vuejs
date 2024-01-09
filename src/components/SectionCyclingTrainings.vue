<template>
    <section class="my_container d-flex mx-auto">
        <div v-for="card in  CyclingTrainings " class="trainings-card">
            <p class="fw-bold">{{ card.name }}</p>
            <img :src="`/src/assets/img/${card.img}`">
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
</style>