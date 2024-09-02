<template>
    <div class="next">
        <a href="#models" class="down" @click="nextPage"><svg xmlns="http://www.w3.org/2000/svg" height="70px" viewBox="0 -960 960 960" width="70px" fill="#e8eaed"><path d="M480-320 216-584l67-67 197 197 197-197 67 67-264 264Z"/></svg></a>
    </div>
</template>

<script>

export default ({
    data() {
        return {
            next: true
        }
    },
    methods: {
        nextPage() {
            this.next = !this.next
            console.log(this.next)
        }
    }
})

</script>

<style scoped>
    .next {
        position: absolute;
        bottom: 50px;
        width: 100%;
        display: flex;
        justify-content: center;
        animation-name: arrow;
        animation-duration: 1s;
        animation-iteration-count: infinite;
    }


    @keyframes arrow {
        0% {
            bottom: 50px;
            opacity: 0;
        } 100% {
            bottom: 20px;
            opacity: 1;
        }
    }
</style>