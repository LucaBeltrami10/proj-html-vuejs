<template>
    <section class="my_container mx-auto text-center">
        <h1>Don't Miss Our Events!</h1>
        <p>Get the amazing cycling experience.</p>
        <div>
            <div class="d-flex justify-content-between">
                <p>Events</p>
                <div class="d-flex">
                    <button>quadratino</button>
                    <button>burghermenu</button>
                </div>
            </div>
            <div class="card-container d-flex">
                <div class="card">
                    <img src="/src/assets/img/event10.jpg" class="card-img-top" alt="...">
                    <div class="card-body text-start">
                        <h1 class="fw-bold fs-6">Toronto Cycling Event 2023</h1>
                        <div class="event-data-info d-flex align-items-center">
                            <i class="fa-regular fa-clock me-1"></i>
                            <p class="m-0">2022-06-22</p>
                            <p class="m-0">01:30</p>
                            <p class="m-0">2023-08-11</p>
                            <p class="m-0">07:00</p>
                        </div>
                        <div class="d-flex">
                            <i class="fa-solid fa-location-dot me-1"></i>
                            <p>Toronto</p>
                        </div>
                        <div class="my_tag">
                            <p>Bicicle Race</p>
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
div.card-container {
    width: calc((100% / 3) - 2rem);
    margin: 1rem 1rem 1rem 1rem;

    p {
        font-size: 0.8rem;
    }

}
</style>