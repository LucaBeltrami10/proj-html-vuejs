<template>
    <section class="my_container mx-auto text-center">
        <div class="my_titles-sections">
            <h1>Don't Miss Our Events!</h1>
            <p>Get the amazing cycling experience.</p>
        </div>
        <div>
            <div class="d-flex justify-content-between mx-2">
                <p>Events</p>
                <div class="d-flex">
                    <button type="button" class="btn btn-light"><i class="fa-solid fa-square"></i></button>
                    <button type="button" class="btn btn-light"><i class="fa-solid fa-bars"></i></button>
                </div>
            </div>
            <div class="card-container d-flex flex-wrap">
                <div v-for="card in EventsInfo" class="my-card card">
                    <img :src="`/src/assets/img/${card.img}`" class="card-img-top" alt="...">
                    <div class="card-body text-start pb-0">
                        <h1 class="fw-bold fs-6">{{ card.title }}</h1>
                        <div class="event-data-info d-flex">
                            <i class="fa-regular fa-clock me-1"></i>
                            <p class="m-0 mb-2">{{ card.startDate }} @ {{ card.startHours }} - {{ card.endDate }} @ {{
                                card.endHours }}</p>
                        </div>
                        <div class="d-flex">
                            <i class="fa-solid fa-location-dot me-1"></i>
                            <p>{{ card.place }}</p>
                        </div>
                        <div class="my_tag">
                            <p class="m-0">{{ card.tag }}</p>
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
        EventsInfo: Object
    }

}
</script>
<style lang="scss">
section.my_container {
    margin-bottom: 5.5rem;

    div.my-card {
        width: calc((100% / 3) - 1.2rem);
        margin: 0.6rem 0.6rem 0.6rem 0.6rem;

        p {
            font-size: 0.7rem;
        }

        i {
            font-size: 0.7rem;
        }

        &:hover {
            box-shadow: rgba(63, 63, 63, 0.2) 0px 8px 24px;
        }

        div.my_tag {
            background-color: rgb(232, 232, 232);
            display: inline-block;
            padding: 0.1rem 0.15rem;
            border-radius: 3px;
            margin-bottom: 0.5rem;

            p {
                font-size: 0.6rem;
            }
        }
    }
}
</style>