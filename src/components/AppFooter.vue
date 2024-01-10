<template>
    <div class="container-fluid pt-4">
        <div class="row">
            <div class="my_left-col col-4 d-flex justify-content-end">
                <div>
                    <img class="mb-3" src="../assets/img/logo-footer-gobike.png" alt="gobike logo's">
                    <div class="d-flex">
                        <i class="fa-solid fa-location-dot me-2"></i>
                        <p>New Jersey, USA</p>
                    </div>
                    <div class="d-flex">
                        <i class="fa-solid fa-phone-volume me-2"></i>
                        <p>+1(234)567 89 10</p>
                    </div>
                    <div class="d-flex">
                        <i class="fa-solid fa-envelope me-2"></i>
                        <p>example@example.com</p>
                    </div>
                    <div class="d-flex mt-1">
                        <button type="button" class="btn btn-dark">
                            <i class="fa-brands fa-facebook-f"></i>
                        </button>
                        <button type="button" class="btn btn-dark mx-1">
                            <i class="fa-brands fa-square-instagram"></i>
                        </button>
                        <button type="button" class="btn btn-dark">
                            <i class="fa-brands fa-twitter"></i>
                        </button>

                    </div>
                </div>
            </div>
            <div class="my_center-col col-4 pe-5">
                <h1 class="fw-bold fs-5">Join Our Newsletter</h1>
                <p class="mb-4">Subscribe to receive usefoul information.</p>
                <div class="my_form">
                    <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="Your Email Address">
                    <button type="button" class="btn btn-light mt-1">Subscribe</button>
                </div>
            </div>
            <div class="my_right-col col-4 d-flex">
                <div v-for="list in footerListEl" class=" me-5">
                    <h1 class="fw-bold fs-6 mb-4">
                        {{ list.listName }}
                    </h1>
                    <ul class="p-0">
                        <li v-for="li in list.options" class="d-flex mb-2">
                            <p class="fw-bold m-0 me-1">-</p>
                            <p class="m-0">{{ li }}</p>
                        </li>
                    </ul>
                </div>

            </div>
        </div>
        <div class="row">
            <div class="col-12 text-center mt-4">
                <p>2022 Gobike - All Right Reserved.</p>
            </div>
        </div>

    </div>
</template>

<script>
export default {
    props: {
        footerListEl: Array,
    },
    data() {
        return {

        }
    },
    methods: {


    },
}
</script>

<style lang="scss">
div.container-fluid {
    background-color: black;
    height: 300px;
    color: white;

    div.row {
        p {
            font-size: 0.7rem;
        }

        div.my_left-col {
            div {
                margin-right: 4rem;

                img {
                    width: 130px;
                }

                button {
                    background-color: black;
                    border-radius: 0;
                }
            }

        }

        div.my_center-col {
            div.my_form {
                input {
                    border-radius: 0;
                    font-size: 0.7rem;
                    height: 2.8rem;
                }

                button {
                    width: 100%;
                    height: 2.8rem;
                    border-radius: 0;
                    font-size: 0.7rem;
                }
            }
        }

        div.my_left-col {}

    }
}
</style>