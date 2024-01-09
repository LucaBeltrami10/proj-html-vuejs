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
                    <img src="..." class="card-img-top" alt="...">
                    <div class="card-body">
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the
                            card's content.</p>
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
div.card-container {}
</style>