<template>
    <div class="home-heading-top">
         <div data-aos="fade-up"  data-aos-easing="linear"
     data-aos-duration="500" class="home-heading-top-inner">
             <h1>
                {{ title }}
            </h1>
             <div class="sub-heading">
                 <p class="sub-heading-text">
                 {{ details }}
                </p>
             </div>
             <a v-if="show" class="btn btn-primary heading-button">ENQUIRE NOW</a>
         </div>
         <div data-aos="fade-up"  data-aos-easing="linear"
     data-aos-duration="500" class="heading-background-image">
         </div>
         <div class="heading-transition"></div>
    </div> 
 </template>

<script>
export default {
    props: [
        'title',
        'details',
        'show'
    ],
    data() {
        return {
            title: this.title,
            details: this.details,
            show: this.show
        }
    }
}
</script>
 
 <style scoped>
 .home-heading-top {
     z-index: 0;
     height: 700px;
     background-image: radial-gradient(circle at 100% 0,#fff,#d9e1f1);
     margin-top: 0;
     padding-top: 160px;
     display: block;
     position: relative;
     top: -88px;
 }
 .home-heading-top-inner{
     z-index: 100;
     max-width: 800px;
     margin: 60px auto 0;
     position: relative;
     top: 0;
 }
 .home-heading-top-inner h1 {
     color: #08083d;
     text-align: center;
     margin-top: 0;
     margin-bottom: 24px;
     font-family: Rubik,Arial,sans-serif;
     font-size: 48px;
     font-weight: 700;
     line-height: 60px;
 }
 
 .sub-heading {
     color: #435b8c;
     text-align: center;
     margin-left: 0;
     margin-right: 0;
     font-family: Rubik,Arial,sans-serif;
     font-size: 16px;
     font-weight: 100;
     line-height: 27px;
 }
 
 .heading-button {
     text-align: center;
     align-self: flex-start;
     margin-top: 32px;
     margin-left: auto;
     margin-right: auto;
     padding-top: 16px;
     padding-bottom: 16px;
     display: block;
     width: 20%;
 }
 
 .heading-background-image {
     transform: translate3d(0px, 0px, 0px) scale3d(1, 1, 1) rotateX(0deg) rotateY(0deg) rotateZ(0deg) skew(0deg, 0deg);
     transform-style: preserve-3d;
     opacity: 1;
     background-image: url('../assets/images/5eaf786185c94f3b6cb57354_bg-image.svg');
     width: 700px;
     height: 700px;
     left: auto;
     z-index: -2;
     background-position: 10px -580px;
     background-repeat: no-repeat;
     background-size: auto;
     position: absolute;
     top: 0%;
     bottom: 0%;
     left: auto;
     right: 0%;
 }
 
 .heading-transition{
     z-index: -99;
     width: 100%;
     height: 200px;
     background-image: linear-gradient(transparent,#fff 78%);
     background-size: auto;
     position: absolute;
     top: auto;
     bottom: 0%;
     left: 0%;
     right: 0%;
 }
 </style>