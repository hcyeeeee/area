<template>
    <div class="layout">
        <!-- <h1>{{ title }}</h1> -->
        <!-- <a href="https://www.ftvnews.com.tw/topics/taiwanghost/" target="blank">
            <picture>
                <source srcset="../assets/banner1920_600.jpg" media="(max-width: 500px)" />
                <source srcset="../assets/banner1920_600.jpg" media="(max-width: 768px)" />
                <source srcset="../assets/banner1920_600.jpg" media="(max-width: 1024px)" />
                <img src="../assets/banner1920_600.jpg" alt="">
            </picture>
        </a> -->

        <div id="carouselExampleCaptions" class="carousel slide computer" data-bs-ride="carousel">
            <div class="carousel-indicators ">
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0"
                    class="active bg-dark" aria-current="true" aria-label="Slide 1"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1"
                    aria-label="Slide 2" class="bg-dark"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2"
                    aria-label="Slide 3" class="bg-dark"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="3"
                    aria-label="Slide 4" class="bg-dark"></button>
            </div>
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <!-- <img src="../assets/banner1920_600.jpg" class="d-block w-100" alt="..."> -->
                    <a href="https://www.ftvnews.com.tw/topics/taiwanghost/" target="blank">
                        <picture>
                            <source srcset="../assets/妖怪1.jpg" media="(max-width: 500px)" />
                            <source srcset="../assets/妖怪2.jpg" media="(max-width: 768px)" />
                            <source srcset="../assets/妖怪3.jpg" media="(max-width: 1024px)" />
                            <img src="../assets/妖怪4.jpg" alt="">
                        </picture>
                    </a>


                    <!-- <div class=" caption d-none d-md-block">
                        <h3>台灣民俗月專題
                        </h3>
                        <p>台灣鬼怪不只林投姐與魔神仔？揭密台灣本土鬼怪傳說</p>
                    </div> -->
                </div>
                <div class="carousel-item">
                    <a href="https://www.ftvnews.com.tw/topics/covid-19/index.html" target="blank">
                        <picture>
                            <source srcset="../assets/暖心1.jpg" media="(max-width: 500px)" />
                            <source srcset="../assets/暖心2.jpg" media="(max-width: 768px)" />
                            <source srcset="../assets/暖心3.jpg" media="(max-width: 1024px)" />
                            <img src="../assets/暖心4.jpg" alt="">
                        </picture>
                    </a>
                </div>
                <div class="carousel-item">
                    <a href="https://www.ftvnews.com.tw/topics/soldier/" target="blank">
                        <picture>
                            <source srcset="../assets/兵役1.jpg" media="(max-width: 500px)" />
                            <source srcset="../assets/兵役2.jpg" media="(max-width: 768px)" />
                            <source srcset="../assets/兵役3.jpg" media="(max-width: 1024px)" />
                            <img src="../assets/兵役4.jpg" alt="">
                        </picture>
                    </a>
                </div>
                <div class="carousel-item">
                    <a href="https://www.ftvnews.com.tw/topics/taiwanghost/" target="blank">
                        <picture>
                            <source srcset="../assets/疫情1.jpg" media="(max-width: 500px)" />
                            <source srcset="../assets/疫情2.jpg" media="(max-width: 768px)" />
                            <source srcset="../assets/疫情3.jpg" media="(max-width: 1024px)" />
                            <img src="../assets/疫情4.jpg" alt="">

                        </picture>
                    </a>
                </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions"
                data-bs-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions"
                data-bs-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Next</span>
            </button>
        </div>

    </div>

</template>

<script>
export default {
    name: 'Intro',
    data() {
        return {
            title: `專題集散區`,
        }
    },
}
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
