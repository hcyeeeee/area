<template>
    <div class="layout_header">
        <div class="layout_grid">
            <!-- logo -->
            <div>
                <p>
                    <img :src="logo" loading="lazy" />
                    <a href="https://www.ftvnews.com.tw/" target="_blank">
                        <span>{{ title }}</span></a>
                </p>
            </div>
            <!-- sharelinks -->
            <a href="https://social-plugins.line.me/lineit/share?url=https://www.ftvnews.com.tw/topics/topicsarea/"
                target="_blank">
                <span id="social_line" data-href="https://www.ftvnews.com.tw/topics/topicsarea/"></span>
            </a>
            <a target="_blank"
                href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fwww.ftvnews.com.tw%2Ftopics%2Ftopicsarea%2F&amp;src=sdkpreparse"
                class="fb-xfbml-parse-ignore"><span id="social_facebook"></span></a>
            <a href=""> <span id="social_link" @click="getLocalUrl"></span></a>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            title: `民視新聞網`,
            logo: require('../assets/logo_ftv.svg'),
            isShow: false,

        }
    },



}
</script>

<style scoped>
a {
    font-weight: 700;
    color: #333;
    filter: contrast(1) !important;
    padding: 10px;
}

.layout_header {
    background-color: #efefef;

    position: fixed;
    width: 100%;
    min-height: 60px;
    box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
    /* box-shadow: rgba(0, 0, 0, 2) 0px 4px 12px; */
    z-index: 9999;

}

.layout_grid {
    grid-template-columns: 9fr 0.5fr 0.5fr 0.5fr;
    font-family: "Noto Sans TC";
}

.layout_menu ul li {
    padding: 1rem 0;
}


#social_line,
#social_facebook,
#social_link {
    display: inline-block;
    background-size: 40px;
    width: 40px;
    height: 40px;
    margin-top: 10px;
    background-repeat: no-repeat;
    border-radius: 10px;
}

#social_line {
    border-radius: 10px;
    background-image: url('../assets/icon_line.png');
}

#social_facebook {
    border-radius: 10px;
    background-image: url('../assets/icon_fb.png');
}

#social_link {
    border-radius: 10px;
    background-image: url('../assets/icon_share.png');
}


p {
    color: #333;
    font-size: 1.7rem;
    text-align: left;
    cursor: default;
    user-select: none;
    display: flex;
    align-items: center;
    margin-top: 5px;

}



p img {
    width: 32px;
    height: 32px;
    margin-top: 5px;
}

span {
    color: #333;
}







@media screen and (max-width: 768px) {

    #social_line,
    #social_facebook,
    #social_link {
        display: inline-block;
        background-size: 35px;
        width: 35px;
        height: 35px;
        background-repeat: no-repeat;
        border-radius: 10px;
    }

    a {
        font-weight: 700;
        color: rgb(22, 22, 22);
        filter: contrast(1) !important;
        padding: 5px;
        padding: 0.3rem;
        margin-right: 10px;
    }

    p {
        margin-top: 4px;
        margin-left: 15px;
    }



}
</style>
