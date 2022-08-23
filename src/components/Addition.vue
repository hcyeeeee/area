<template>
    <div class="layout_addition" @scroll="scroll">
        <div class="layout_grid">
            <a href="https://social-plugins.line.me/lineit/share?url=https://www.ftvnews.com.tw/topics/topicsarea/"
                target="_blank">
                <span id="social_line" data-href="https://www.ftvnews.com.tw/topics/topicsarea/"></span>
            </a>

            <a target="_blank"
                href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fwww.ftvnews.com.tw%2Ftopics%2Ftopicsarea%2F&amp;src=sdkpreparse"
                class="fb-xfbml-parse-ignore"><span id="social_facebook"></span></a>
            <span id="social_link" @click="getLocalUrl"></span>
        </div>
        <!-- <div v-if="scrollY > 100">
            <i @click="scrollTop" id="toTop" class="fa-solid fa-square-arrow-up fa-3x"></i>
        </div> -->
    </div>
</template>

<script>
export default {
    data() {
        return {
            scrollY: '',
        }
    },
    methods: {
        getLocalUrl() {
            let e = document.createElement('input'),
                t = window.location.href + '?utm_source=topicsarea&utm_medium=copybutton'
            document.body.appendChild(e),
                (e.value = t),
                e.select(),
                document.execCommand('copy'),
                document.body.removeChild(e),
                alert('網址複製成功!')
        },

        scrollTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' })
        },

        scroll() {
            this.scrollY = window.scrollY
        },
    },
    created() {
        window.addEventListener('scroll', this.scroll)
    },
}
</script>

<style scoped>
.layout_addition {
    height: 100px;
}

.layout_grid {
    grid-template-columns: 1fr 1fr 1fr;
    max-width: 300px;
    padding: 1rem;
}

a,
span {
    display: block;
    margin: auto;
    cursor: pointer;
    filter: contrast(1);
}

a:hover {
    background-color: #ffffff00;
}

.addition {
    position: fixed;
    top: 5%;
    right: 1px;
    border-radius: 15px;
    padding: 10px 5px;
    background-color: #f7f7f5;
    box-shadow: 1px 2px 3px black;
    z-index: 999;
}

#social_line,
#social_facebook,
#social_link {
    display: block;
    background-size: 40px;
    width: 40px;
    height: 40px;

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

.fa-square-arrow-up {
    position: fixed;
    right: 1rem;
    bottom: 4rem;
    z-index: 9999;
    color: #162237;
    opacity: .8;
}
</style>
