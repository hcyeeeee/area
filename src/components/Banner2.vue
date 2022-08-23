<template>
    <div class="layout">
        <carousel>

            <img src="https://placeimg.com/200/200/any?1">

            <img src="https://placeimg.com/200/200/any?2">

            <img src="https://placeimg.com/200/200/any?3">

            <img src="https://placeimg.com/200/200/any?4">

        </carousel>
    </div>

</template>

<script>
import carousel from 'vue-owl-carousel'
export default {
    components: { carousel },
}
$(".owl-carousel").owlCarousel({
    loop: true, // 循環播放
    margin: 10, // 外距 10px
    nav: true, // 顯示點點
    responsive: {
        0: {
            items: 1 // 螢幕大小為 0~600 顯示 1 個項目
        },
        600: {
            items: 3 // 螢幕大小為 600~1000 顯示 3 個項目
        },
        1000: {
            items: 5 // 螢幕大小為 1000 以上 顯示 5 個項目
        }
    }
});

</script>



<style scoped>
.layout {
    background-color: #efefef;
    padding: 2rem;
    width: 100%;
    min-height: 200px;
    /* background: linear-gradient(to bottom, white, #e6e6e6); */
}

img {

    pointer-events: none;
    margin: 6rem auto 3rem;

}

.carousel .carousel-inner {
    max-width: 1000px;
    margin: auto;

}

.slide {
    max-width: 1000px;
    margin: auto;

}

.carousel-item {}

h1 {
    position: absolute;
    opacity: 0;
}

/* .caption {

    background-color: #d2e0dc;
    padding: 2rem;
    top: 30px;
    width: 30px;
    height: 30px;
    position: absolute;
} */
</style>
