<template>
    <div class="model">
        <h2>BMW Models</h2>
        <div class="model-content">

            <div class="model-detail" v-for="image in images" :key="image.id">
                <img :src="image.src" alt="BMW Model">
                <div class="cars-detail">
                    <h3>{{ image.name }}</h3>
                    <p>
                        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nesciunt dolorum adipisci architecto odio excepturi odit fugiat rem! Molestiae similique blanditiis sapiente sint id totam amet illum, fuga aliquam in, dolor pariatur voluptatem architecto nulla corporis, suscipit corrupti necessitatibus aspernatur animi. Tempora molestiae eaque quam magnam quis, nobis veritatis voluptate id quo dolorum, nostrum dolorem facilis itaque, deserunt blanditiis exercitationem et reiciendis perferendis molestias? Praesentium, veniam alias. Repudiandae eum tenetur atque!
                    </p>
                </div>
            </div>

        </div>
    </div>
</template>

<script>
export default ({
    data() {
        return {
            images: [
                {id: 1, src: '/img/model1.675d17a6.png', name: 'BMW E class'},
                {id: 2, src: '/img/model2.7ad4b98c.png', name: 'BMW G class'},
                {id: 3, src: '/img/model3.de57843e.png', name: 'BMW M class'},
                {id: 4, src: '/img/model4.07088590.png', name: 'BMW X class'},
            ]
        }

    }
})
</script>

<style scoped>
    .model {
        width: 100%;
        background-color: rgba(0, 0, 0, 0.7);

    }

    h2 {
        text-align: center;
        color: #fff;
        font-size: 3rem;
        padding: 2rem;
    }

    h3 {
        margin-bottom: 2rem;
    }
    
    .model-detail {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .model-detail img {
        width: 500px;
        margin-right: 3rem;
        animation-name: model;
        animation-duration: 1.5s;
    }

    @keyframes model {
        0% {
            opacity: 0;
            transform: translateX(-100px);
        }100% {
            opacity: 1;
            transform: translateX(0);
        }
    }

    .model-detail img:hover {
        cursor: pointer;
        transform: scale(1.05);
    }

    .cars-detail {
        padding: 1rem;
        background-color: #333;
        opacity: 0.8;
        width: 50%;
        text-align: center;
        color: #fff;
        border-radius: 10px;
        animation-name: detail;
        animation-duration: 1.5s;
    }

    @keyframes detail {
        0% {
            opacity: 0;
            transform: translateX(100px);
        }100% {
            opacity: 1;
            transform: translateX(0);
        }
    }

    .cars-detail p {
        line-height: 1.5;
    }
</style>
