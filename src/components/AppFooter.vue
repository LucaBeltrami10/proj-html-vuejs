<template>
    <div class="container-fluid pt-5">
        <div class="row">
            <div class="my_left-col col-4 d-flex justify-content-end">
                <div>
                    <img src="../assets/img/logo-footer-gobike.png" alt="gobike logo's">
                    <div class="d-flex">
                        <p>New Jersey, USA</p>
                    </div>
                    <div class="d-flex">
                        <p>+1(234)567 89 10</p>
                    </div>
                    <div class="d-flex">
                        <p>example@example.com</p>
                    </div>
                    <div class="d-flex">
                        <button type="button" class="btn btn-dark">D</button>
                        <button type="button" class="btn btn-dark mx-1">D</button>
                        <button type="button" class="btn btn-dark">D</button>
                    </div>
                </div>
            </div>
            <div class="my_center-col col-4 pe-5">
                <h1 class="fw-bold fs-5">Join Our Newsletter</h1>
                <p>Subscribe to receive usefoul information.</p>
                <div class="my_form">
                    <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="Your Email Address">
                    <button type="button" class="btn btn-light mt-1">Subscribe</button>
                </div>
            </div>
            <div class="my_right-col col-4 d-flex">
                <ul>
                    <li>prova</li>
                </ul>
                <ul>
                    <li>prova</li>
                </ul>
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
                    width: 120px;
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