<template>
    <section class="my_container mx-auto mb-5">
        <div class="text-center">
            <h1>Recent New & Articles</h1>
            <p>important informatios about bike</p>
        </div>
        <div class="card_container d-flex">
            <div v-for="article in newArticles" class="my_card text-center">
                <img :src="`/src/assets/img/${article.img}`" :alt="`${article.subject} photo's `">
                <p class="fw-bold data_news">{{ article.data }} - {{ article.subject }}</p>
                <h1 class="fw-bold fs-6">{{ article.title }}</h1>
                <p>{{ article.preview }}]</p>
                <button type="button" class="btn btn-dark">More</button>
            </div>
        </div>

    </section>
</template>
<script>
export default {
    props: {
        newArticles: Array
    }

}
</script>
<style lang="scss" scoped>
section.my_container {
    div.card_container {
        div.my_card {
            width: calc((100% / 4) - 2.4rem);
            margin: 0 1.2rem;
            padding: 1rem;
            border-radius: 5px;
            box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;

            p {
                font-size: 0.6rem;

                &.data_news {
                    font-size: 0.7rem;
                }
            }

            img {
                width: 100%;
            }

            button {
                padding: 0.8rem 1.5rem;
                border-radius: 3px;
                font-size: 0.7rem;
                font-weight: bold;
            }
        }
    }
}
</style>