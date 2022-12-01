<template>
 <section class="hero">
  <div class="container">
   <div class="hero-wrap">
    <div class="hero-content">
      <h1>Be part of the community</h1>
      <p class="hero-descr">It should be noted that the further development of various 
       forms of activity is a qualitatively new stage in the analisis 
       of existing patterns of behavior</p>
     <Button class="hero-btn" text="Start Membership"/>
     <h2>BeePro</h2>
     <div class="hero-card">
      <div></div>
      <img :src="heroBee" alt="bee">
     </div>
    </div>
    <div class="hero-content-mobile">
      <img :src="heroBeeMobile" alt="bee"/>
      <h3>Welcome to beepro</h3>
      <p>
        It should be noted that the further 
        <br>
        development of various forms 
        <br>
        of activity is a qualitatively new stage 
        <br>
        in the analisis of existing patterns
        <br>
        of behavior
      </p>
      <Button class="hero-btn" text="Start Membership"/>
    </div>
    <span class="light light-blue"></span>
    <span class="light light-orange"></span>
    <span class="light light-yellow"></span>
   </div>
  </div>
 </section>
</template>


<script>
import Button from './buttons/Button'
import heroBee from '@/assets/images/bee.png'
import heroBeeMobile from '@/assets/images/bee-mobile.png'

export default {
  components: {
   Button
  },
  data: () => {
   return {
    heroBee,
    heroBeeMobile
   }
  }
}
</script>

<style>
 .hero-wrap {
  padding: 221px 0 86px;
 }

 .hero-wrap, .hero h1, .hero h2, .hero-descr, .hero-btn {
  position: relative;
  z-index: 20;
 } 

 .hero::before {
  position: absolute;
  content: '';
  width: 80%;
  height: 100%;
  background:radial-gradient(98.05% 261.61% at 1.95% 3.59%, rgba(255, 255, 255, 0.4) 0%, rgba(255, 255, 255, 0) 100%);
  backdrop-filter: blur(40px);
  border-radius: 0px 0px 56px 0px;
  box-sizing: border-box;
  border-image: linear-gradient( rgba(255, 255, 255, 0), rgba(255, 255, 255, 0.4)) 0;
  border-width: 2px;
  border-style: solid;
  z-index: 10;
 }

 .hero h1 {
  font-weight: 700;
  font-size: var(--fz-64);
  line-height: 130%;
  text-transform: uppercase;
  font-feature-settings: 'pnum' on, 'lnum' on;
  max-width: 608px;
 }

 .hero-descr {
  margin-top: 20px;
  font-weight: 500;
  line-height: 160%;
  max-width: 480px;
 }

 .hero-btn {
  margin-top: 30px;
 }

 .hero h2 {
  margin-top: 61px;
  font-weight: 700;
  font-size: var(--fz-48);
  line-height: 130%;
  text-transform: capitalize;
  font-feature-settings: 'pnum' on, 'lnum' on;
  color: var(--special-color);
 }

 .hero-card {
  position: absolute;
  width: 521px;
  height: 691px;
  background: radial-gradient(209.87% 161.91% at 70.19% 100%, rgba(255, 255, 255, 0.4) 0%, rgba(255, 255, 255, 0) 100%);
  backdrop-filter: blur(40px);
  border-radius: 0px 0px 56px 0px;
  top: 168px;
  right: 99px;
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 40;
 }

 .hero-card div {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0; 
 }

 .hero-card div::before {
  content: '';
  position: absolute;
  right: 0;
  width: 2px;
  height: 100%;
  background: linear-gradient(rgba(255, 255, 255, 0.4), rgba(255, 255, 255, 0)) 0;
  z-index: 50;
 }

 .hero-card::before {
  content: '';
  position: absolute;
  left: 0;
  width: 2px;
  height: 100%;
  background: linear-gradient(rgba(255, 255, 255, 0.4), rgba(255, 255, 255, 0)) 0;
  z-index: 50;
 }

 .hero-card::after {
  content: '';
  position: absolute;
  top: 0;
  width: 100%;
  height: 2px;
  background: rgba(255, 255, 255, 0.4);
  z-index: 50;
 }

 .hero-card img {
  position: absolute;
  object-fit: contain;
  width: 100%;
  height: auto;
  z-index: 30;
 }

 .hero-content-mobile {
  display: none;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: relative;
  z-index: 20;
 }

 .hero-content-mobile h3 {
  font-weight: 700;
  font-size: 5.4vw;
  text-transform: uppercase;
  font-feature-settings: 'pnum' on, 'lnum' on;
 }

 .hero-content-mobile p {
  margin-top: 2.8vw;
  font-weight: 500;
  font-size: 3vw;
  line-height: 160%;
  text-align: center;
 }

 .hero-content-mobile .button {
  border-radius: 11px;
  font-size: 10px;
  padding: 10px 27px;
 }

 .hero .light.light-blue {
  width: 26vw;
  height: 28vw;
  top: 77px;
  left: 60%;
 }

 .hero .light.light-orange {
  width: 22vw;
  height: 22vw;
  left: -109px;
  top: -133px;
 }

 .hero .light.light-yellow {
  width: 22vw;
  height: 6vw;
  left: 14%;
  top: 515px;
 }
</style>