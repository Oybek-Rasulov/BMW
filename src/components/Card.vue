<template>
    <div class="container">
        <div class="card" v-if="card">
            <v-card
                class="mx-auto"
                max-width="344">
                <v-card-text>
                    <div class="card-title">
                        <h3>BMW M8</h3>
                        <button class="close-btn" @click="toggleClose"><svg xmlns="http://www.w3.org/2000/svg" height="25px" viewBox="0 -960 960 960" width="48px" fill="#F3F3F3"><path d="m249-207-42-42 231-231-231-231 42-42 231 231 231-231 42 42-231 231 231 231-42 42-231-231-231 231Z"/></svg></button>
                    </div>

                    <p class="text-h4 font-weight-black mb">High-performance version of new generation</p>

                    <div class="details">
                        <p class="card-info mb">Speed</p>
                        <div class="line" style="width: 70%"></div>
                    </div>

                    <div class="details">
                        <p class="card-info mb">Compfort</p>
                        <div class="line" style="width: 60%"></div>
                    </div>

                    <div class="details">
                        <p class="card-info mb">Endurance</p>
                        <div class="line" style="width: 40%"></div>
                    </div>

                    <div class="details">
                        <p class="card-info mb">Quality</p>
                        <div class="line" style="width: 50%"></div>
                    </div>

                </v-card-text>

                <v-card-actions>
                <v-btn
                    color="deep-purple-accent-4"
                    text="Learn More"
                    variant="text"
                ></v-btn>
                </v-card-actions>
            </v-card>
        </div>
    </div>
</template>

<script>

export default ({
    data() {
        return {
            card: true
        }
    },
    methods: {
        toggleClose() {
            this.card = false;
        }
    }
})
</script>

<style scoped>

    .container {
        display: flex;
        justify-content: flex-end;
    }

    .card {
        width: 500px;
        background-color: rgba(255, 255, 255, 0.3);
        color: #fff;
        padding: 2rem 3rem;
        border-radius: 10px;
        font-weight: bold;

        /* animation */
        animation-name: card;
        animation-duration: 1.5s;
        animation-iteration-count: initial;


    }

    @keyframes card {
        0% {
            transform: translateX(300px);
            opacity: 0;
        }
        100% {
            transform: translateX(0);
            opacity: 1;
        }
    }

    .mb {
        margin: 0 1rem 1rem 0 ;
    }

    .card-title {
        display: flex;
        justify-content: space-between;
        align-items: center;
        font-size: 1.5rem;
        margin-bottom: 2rem;

    }

    .details {
        display: flex;
        align-items: center;
        justify-content: space-between;
    } 

    .line {
        width: 30%;
        height: 5px;
        background-color: yellow;
        border-radius: 5px;
        margin-bottom: 1rem;
    }

</style>
