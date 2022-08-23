<template>
    <div id="app">

        <Header />

        <Banner />
        <Section />
        <Section1 />
        <Addition />
        <Footer />
    </div>
</template>



<script>
import Header from '@/components/Header.vue'
import Banner from '@/components/Banner.vue'
import Section from '@/components/Section.vue'
import Section1 from '@/components/Section1.vue'
import Addition from '@/components/Addition.vue'
import Footer from '@/components/Footer.vue'


export default {
    name: 'App',
    components: {
        Header,
        Section,
        Banner,

        Section1,
        Addition,
        Footer,
    },
}

</script>


<style>
@import url("https://fonts.googleapis.com/css?family=Noto+Sans+TC:wght@100;300&display=swap");
@import url('https://fonts.googleapis.com/css2?family=Noto+Serif+TC:wght@500;600;700&display=swap');



html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;

}

/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
    display: block;
}

a {
    color: black;
    text-decoration: none;
    display: block;
    transition: 0.3s;

}

/* a:hover {
    filter: contrast(1);
} */

i {
    cursor: pointer;
}

body {
    line-height: 1.4;
}

ol,
ul {
    list-style: none;
}

blockquote,
q {
    quotes: none;
}

blockquote:before,
blockquote:after,
q:before,
q:after {
    content: '';
    content: none;
}

table {
    border-collapse: collapse;
    border-spacing: 0;
}

h3,
h4,
p {
    font-size: 16px;
    line-height: 1.56;
}

#app {

    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    background-color: white;
    background-color: #efefef;
    background: linear-gradient(to bottom, white, #efefef, white);
    color: #2f2f2f;
}
</style>

<style>
* {
    scroll-behavior: smooth;
}

p {
    font-size: 1.2rem;
}

h2 {
    text-align: center;
    font-size: 1.8rem;

    font-weight: bold;
    letter-spacing: 0.3rem;

}

h3 {
    /* display: -webkit-box;
    overflow: hidden;
    font-size: 1.2rem;
    text-align: left;
    text-overflow: ellipsis;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    line-height: 30px;
    max-height: 50px;
    margin: auto;
    margin-bottom: 2rem; */
    overflow: hidden;
    font-size: 1.2rem;
    line-height: 30px;


}

h4 {
    display: -webkit-box;
    overflow: hidden;
    font-size: 1.2rem;
    text-align: left;
    text-overflow: ellipsis;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    line-height: 30px;
    max-height: 55px;
    margin: auto;
    padding-left: 0.5rem;
}

img,
picture {
    width: 100%;
    height: auto;
}

.btn_more {
    margin-top: 3rem;
}

.fa-solid {
    color: #525b7c;
}

.layout {
    margin: auto;
}

.layout_grid {
    max-width: 1000px;
    margin: auto;
    display: grid;
    /* padding: 4.1rem 1rem; */
}

#section_news,
#section1,
#section2,
#section3 {
    min-height: 500px;
}

@media screen and (max-width: 768px) {

    #section_news,
    #section1,
    #section2,
    #section3 {
        min-height: 500px;
    }
}

.layout_inner .layout_photo p {
    text-align: left;
    font-size: 1rem;
    padding: 1rem 3rem 2rem !important;
}

/* 4x3 縱橫比 */
.iframe-container {
    overflow: hidden;
    padding-top: 56.25%;
    position: relative;
    margin-top: 3rem;
    z-index: 1;
    width: 100%;
    min-height: 100px;
}

.iframe-container iframe {
    border: 0;
    height: 100%;
    left: 0;
    position: absolute;
    top: 0;
    width: 100%;
}

.iframe-container-4x3 {
    padding-top: 75%;
}
</style>
