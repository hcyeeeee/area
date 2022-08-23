<template>
    <div class="layout">
        <picture>
            <source srcset="../assets/數位專題集散地-04.jpg" media="(max-width: 768px)" />
            <source srcset="../assets/數位專題集散地-03.jpg" media="(max-width: 1024px)" />
            <img src="../assets/數位專題集散地-02.jpg" alt="數位專題集散地">
        </picture>
        <!-- <h2>民視新聞&nbsp;數位專題</h2> -->
    </div>

</template>



<style scoped>
.layout {

    background-size: cover;
    background-color: #d8dedd;
    /* padding: 2rem 0rem 0rem; */
    /* max-width: 1000px; */
}



img {
    margin: auto;
    max-width: 1000px;
}


@media screen and (min-width: 768px) {
    img {
        margin: auto;
        width: 100%;
    }

}
</style>
