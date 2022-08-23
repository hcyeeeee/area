<template>
    <div class="layout" id="section1">
        <div class="layout_grid" v-for="(item, index) in anchor" :key="index">
            <a :href="'https://www.ftvnews.com.tw/topics/' + item.id" target="blank">
                <div class="layout_grid_inner ">


                    <div class=" layout_img">
                        <img class="m" v-bind:src="item.urlm" loading="lazy" alt=item.id />
                        <img class="c" v-bind:src="item.url" loading="lazy" alt=item.id />
                    </div>


                    <div class="layout_content">
                        <h2>{{ item.topictitle }}</h2>
                        <h3>{{ item.subtitle }}</h3>

                    </div>

                    <div class="layout_content2">

                        <p class="m" v-html="item.contentm"></p>
                        <p class="c" v-html="item.content"></p>

                    </div>
                </div>


            </a>



        </div>

    </div>
</template>

<script>
export default {
    data() {
        return {
            title: `民視數位專題`,
            newsInfo: [],



            anchor: [
                {
                    topictitle: '最新疫情專區',
                    subtitle: '【最新疫情】快篩陽了怎麼辦？確診隔離指引、疫情動態這邊看',
                    contentm: '受到變種病毒Omicron侵襲，全球爆發新一波武漢肺炎（新冠肺炎、COVID-19）疫情，國內本土確診數也不斷飆高民視新聞特別製作數位專題，運用各式圖表......',
                    content: '受到變種病毒Omicron侵襲，全球爆發新一波武漢肺炎（新冠肺炎、COVID-19）疫情，國內本土確診數也不斷飆高。<br>民視新聞特別製作數位專題，運用各式圖表，提供「台灣疫情整理」、「最新疫苗資訊」、「快篩實名制Q&A」等，讓讀者能即時掌握疫情資訊。',
                    id: `covid-19/index.html`,
                    pic: `covid`,
                    urlm: require('../assets/疫情2.jpg'),
                    url: require('../assets/疫情3.jpg')
                },
                {
                    topictitle: '暖新聞專區',
                    subtitle: '暖新聞專區｜療癒毛孩、抗疫故事、勵志人物、國際暖聞、公益送暖',
                    contentm: '近日身處在疫情延燒、俄烏戰爭未見停歇、通膨風暴席捲全球的生活中，是否令你感到焦慮不安？或是高壓忙碌的工作，讓你感覺身心俱疲？雖然日常生活裡，我們偶爾......',
                    content: '近日身處在疫情延燒、俄烏戰爭未見停歇、通膨風暴席捲全球的生活中，是否令你感到焦慮不安？或是高壓忙碌的工作，讓你感覺身心俱疲？<br>雖然日常生活裡，我們偶爾會低潮、憂鬱，但別忘了這個世界還是有很多好事發生！民視新聞網替大家精選療癒、正向暖新聞，希望為世界帶來一點正能量，鼓舞每個人帶著溫暖的心，繼續向前行。',
                    id: `warm`,
                    urlm: require('../assets/暖心2.jpg'),
                    url: require('../assets/暖心3.jpg'),
                },
                {
                    topictitle: '台灣兵役專題',
                    subtitle: '兵役延長助台灣國防？現代戰爭人海戰術還有效嗎？',
                    contentm: '俄羅斯入侵烏克蘭，讓台海安全備受關注，不少民眾也開始檢討現行4個月軍事訓練役制度，是否能培養出有戰力的後備軍人？還是該恢復1年役期？延長兵役......',
                    content: '俄羅斯入侵烏克蘭，讓台海安全備受關注，不少民眾也開始檢討現行4個月軍事訓練役制度，是否能培養出有戰力的後備軍人？還是該恢復1年役期？延長兵役、增加役男人數，就能夠強化國防安全嗎？<br>民視新聞網專訪到《阿共打來怎麼辦》作者王立，從俄烏戰爭切入，分析台灣兵役制度以及「不對稱作戰」優勢在哪裡，並製成數位專題，以Q&A、圖表形式幫助大家理解。',
                    id: `soldier/`,
                    urlm: require('../assets/兵役2.jpg'),
                    url: require('../assets/兵役3.jpg'),
                },
                {
                    topictitle: '台灣民俗月專題',
                    subtitle: '台灣鬼怪不只林投姐與魔神仔？揭密台灣本土鬼怪傳說',
                    contentm: '你知道台灣也有自己的鬼怪文化嗎？民視新聞網特別製作台灣民俗月專題，用心理測驗跟專家訪談介紹台灣的本土文化、揭密台灣豐富的妖怪傳說。',
                    content: '你知道台灣也有自己的鬼怪文化嗎？民視新聞網特別製作台灣民俗月專題，用心理測驗跟專家訪談介紹台灣的本土文化、揭密台灣豐富的妖怪傳說。',
                    id: `taiwanghost`,
                    urlm: require('../assets/妖怪2.jpg'),
                    url: require('../assets/妖怪3.jpg'),

                },

            ],


        }
    },

    mounted() {
        // eslint-disable-next-line no-undef

    },
}
</script>

<style scoped>
.layout {

    /* background: linear-gradient(to bottom, #d8dedd, #efefef); */
    /* background-image: linear-gradient(to right bottom, #ffffff, #c7dced); */
}

.layout_img {
    margin: auto;

}

.layout_img_inner {

    cursor: pointer;

}

img {
    border-radius: 10px 0px 0px 10px;

}

.layout_grid {
    margin: 3rem auto;


}

.layout_grid_inner {
    display: grid;
    background-color: white;
    grid-template-columns: 4fr 3fr;
    grid-gap: 1rem;
    box-shadow: rgba(0, 0, 0, 0.08) 0px 4px 12px;
    cursor: pointer;
    opacity: .9;
    border-radius: 10px;
    border-radius: 10px;

}

.layout_content {
    padding: 0rem 1.5rem;
    margin: auto;
}

@media screen and (min-width: 768px) {
    .layout_content2 {
        display: none;
    }

    .layout_grid_inner:hover .layout_content2 {
        display: block;
        padding: 1.5rem;
        margin: auto;
        transition: 2s linear;
        opacity: .9;
    }

    .layout_grid_inner:hover .layout_content {
        display: none;
    }


    .layout_grid_inner:hover {
        transition: 200ms linear;
        /* transition: 1s ease; */
        background-color: #efefef;
        background-color: white;
        color: #2a2a2a;
        transform: scale(1.01);
        opacity: 1;
        box-shadow: rgba(17, 17, 26, 0.1) 0px 4px 16px, rgba(17, 17, 26, 0.05) 0px 8px 32px;
    }

    .layout_img:hover {
        margin: auto;
        height: 100%;
        padding: 0rem;

    }

    .layout_img {
        padding: 0rem;
    }


    h3 {
        text-align: left;
        font-size: 1.3rem;
        font-weight: 700;
        line-height: 2.2rem;
    }

    h2 {

        font-style: none;
        font-size: 2.3rem;
        text-align: left;
        line-height: 3rem !important;
        font-weight: bold;
        padding: 0.5rem 0rem;
    }

    i {
        display: flex;
        padding: 1rem;
        justify-content: end;
        color: #333;
    }

    .m {
        display: none;
    }


}



@media screen and (max-width: 768px) {
    .layout_grid_inner {
        grid-template-columns: 1fr;
        margin: 1.5rem 2rem;
        padding: 1rem;
    }

    h2 {
        display: none;
    }

    h3 {
        padding: 0rem;
        font-size: 1.6rem;
        line-height: 2.4rem;
        font-weight: 600;
        text-align: left;
    }

    .layout_content {
        padding: 0rem;
        margin: auto;
    }

    .layout_content2 {
        padding: 0rem;
        margin: auto;
    }

    i {
        display: none;
    }

    img {
        border-radius: 10px;

    }

    .layout_grid {
        margin: 1rem auto;


    }

    .c {
        display: none;
    }

    .m {
        display: block;
    }
}


.btn_more {
    margin-top: 3rem;
}

p {
    text-align: left;
    font-size: 1.2rem;
    line-height: 2rem;
    font-weight: 700;
}


a {
    text-decoration: none;
    color: #333;
}
</style>
