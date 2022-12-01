<template>
  <!-- <div id="app" @contextmenu="handler($event)"> -->
  <div id="app">
    <Header />
    <Hero />
    <Teaser />
    <Beendexer />
    <Functions />
    <Tocenomics/>
    <Collection/>
    <Roadmap />
    <Contact/>
    <Subscribe />
    <Footer /> 
  </div>
</template>

<script>
import Header from './components/Header'
import Hero from './components/Hero'
import Teaser from './components/Teaser'
import Beendexer from './components/Beendexer'
import Functions from './components/Functions'
import Tocenomics from './components/Tocenomics'
import Collection from './components/Collection'
import Roadmap from './components/Roadmap'
import Contact from './components/Contact'
import Subscribe from './components/Subscribe'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Teaser,
    Beendexer,
    Functions,
    Tocenomics,
    Collection,
    Roadmap,
    Contact,
    Subscribe,
    Footer
  },
  methods: {
    handler: function(e) {
        e.preventDefault();
        alert('=)')
    }
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600&display=swap");


:root {
  /* colors */

 --color-body: #1c1c1c;
 --color-white: #FFFFFF;
 --black-color: #000000;
 --grey-color:#E7E7E7;
 --second-grey-color:#D9D9D9;
 --special-color: #FFDD2C;
 --text-input-color:#818181;
 

  /* font-size */

 --fz-14: 14px;
 --fz-16: 16px;
 --fz-22: 22px;
 --fz-24: 24px;
 --fz-32: 32px;
 --fz-48: 48px;
 --fz-55: 55px;
 --fz-64: 64px;
}

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  color: var(--color-white);
  font-family: "Montserrat", sans-serif;
  font-size: var(--fz-16);
}

a {
  text-decoration: none;
  cursor: pointer;
}
li {
  list-style-type: none;
}
ul {
  margin-left: 0;
  padding-left: 0;
}
body {
  background: var(--color-body);
}

section {
  position: relative;
}

input:focus,
input:active,
button:focus,
button:active {
  outline: none;
}


.container {
  padding: 0 100px;
}

.light {
  position: absolute;
  z-index: 5;
  border-radius: 100%;
}

.light.light-blue {
  background: #085575;
  opacity: 0.8;
  filter: blur(200px);
}

.light.light-orange {
  background: #f78d2e;
  filter: blur(200px);
}

.light.light-yellow {
  background: #ffdd2c;
  filter: blur(140px);
}

@media (max-width: 1439px) {
 :root {
  --fz-14: calc(10px + (4 + 4 * 0.3) * ((100vw - 375px) / 1440));
  --fz-16: calc(14px + (2 + 2 * 0.3) * ((100vw - 375px) / 1440));
  --fz-22: calc(14px + (8 + 8 * 0.3) * ((100vw - 375px) / 1440));
  --fz-25: calc(18px + (6 + 6 * 0.3) * ((100vw - 375px) / 1440));
  --fz-32: calc(22px + (10 + 10 * 0.3) * ((100vw - 375px) / 1440));
  --fz-48: calc(32px + (26 + 26 * 0.3) * ((100vw - 375px) / 1440));
  --fz-55: calc(24px + (31 + 31 * 0.3) * ((100vw - 375px) / 1440));
  --fz-64: calc(28px + (36 + 36 * 0.3) * ((100vw - 375px) / 1440));
 }

 .container {
    padding: 0 60px;
  }

  header nav li {
  padding: 0 10px;
 }

 .login {
  padding: 0 0 0 20px;
 }

 .hero-card {
  right: 0;
  width: calc(260px + (261 + 261 * 0.65) * ((100vw - 540px) / 1440));
  height: 691px;
  height: calc(260px + (345 + 345 * 0.65) * ((100vw - 540px) / 1440));
  top: 200px;
 }

 .hero-wrap {
  padding: 150px 0 50px;
 }

 .teaser {
  padding: 14vw 0 7vw;
 } 

 .beendexer {
    padding: 7vw 0 4vw;
 }

 .functions {
    padding: 4vw 0 3vw;
 }

 .functions-content {
    margin-top: 8vw;
  }


 .functions-content div:nth-child(1) img {
    width: 140%;
    height: 140%;
 }

 .functions-content div:nth-child(2) .functions-cells {
  position: absolute;
  width: 44vw;
  height: 44vw;
  bottom: -100px;
  left: 37%;
 }

 .functions-cell p {
    font-size: .9vw;
 }

 .functions h4{
    margin-top: 20vw;
 }

 .functions-items {
  max-width: 100%;
 }

 .collection-card {
  height: 462px;
  width: 309px;
 }

 .collection-card-preview {
  width: 100%;
  height: 296px;
 }

 .collection-card-descr {
  top: 240px;
  width: 100%;
  height: 223px;
  padding: 78px 36px 0;
 }

 .collection-name {
  font-size: 14px;
  margin-top: 14px;
 }

 .collection-autor, .collection-data span {
  font-size: 10px;
 } 

 .collection-autor-avatar {
    width: 20px;
    height: 20px;
  }

  .collection-data {
    margin-top: 16px;
  }
  .collection-data p {
    font-size: 14px;
  }

  .collection-data div:nth-child(2) {
    margin-top: 16px;
  }

  .contact {
    position: relative;
    padding-top: 6vw;
    margin: 0 auto 2vw;
    max-width: 60vw;
    max-height: 70vw;
  }

  .contact img {
    bottom: 1vw;
    right: 1vw;
    height: 364px;
    width: 275px;
  }

 .subscribe {
    padding: 8vw 0 6vw;
  }
  
  footer {
  height: 398px;
  padding: 40px;
  }
}

@media (max-width: 1289px) {

  header nav li span, nav li a {
    font-size: 1.2vw;
  }

  .connect-btn {
    font-size: 8px;
  }

  .button {
    padding: 10px 18px;
  }

  .connect {
    padding: 0;
  }

  .hero-descr {
    max-width: 324px;
  }

  .hero h1 {
    font-size: 3vw;
  }

  .hero-card img {
    width: 75%;
  }

  .functions-items {
    margin: 60px auto 0;
    height: auto;
    display: grid;
    gap: 38px;
    grid-template: repeat(3, 1fr) / 100%;
  }

  .functions-item {
    padding: 40px;
  }

  .contact img {
    bottom: 4vw;
    right: 2vw;
    height: 254px;
    width: 192px;
  }
}

@media (max-width: 1059px) {
  :root {
  --fz-48: 28px;
  --fz-64: 34px;
  }

  .functions h4, .beendexer h3 {
    font-size: 30px;
  }

  .beendexer-card {
    padding: 60px 40px;
  }

  .functions-item {
    padding: 20px;
  }

  .tocenomics-btn {
    font-size: 20px;
    padding: 10px 30px;
  }

  .collection {
    padding: 8vw 0 2vw;
  }

  .collection-card {
  height: 323px;
  width: 216px;
 }

 .collection-card-preview {
  width: 100%;
  height: 207px;
 }

 .collection-card-descr {
  top: 168px;
  width: 100%;
  height: 156px;
  padding: 56px 26px 0;
 }

 .collection-name {
  font-size: 12px;
  margin-top: 10px;
 }

 .collection-autor span, .collection-data span {
  font-size: 10px;
 } 

 .collection-autor-avatar {
    width: 16px;
    height: 16px;
  }

  .collection-data {
    margin-top: 10px;
  }
  .collection-data p {
    font-size: 10px;
  }

  .collection-data div:nth-child(2) {
    margin-top: 8px;
  }

  .functions-item p {
    margin-top: 16px;
  }

  .subscribe h3 {
    max-width: 100%;
  }

  .subscribe-card {
    padding: 40px;
  }

  .collection-content {
    margin: 80px auto 20px;
  }

  .contact img {
    bottom: 8vw;
    right: 2vw;
    height: 177px;
    width: 133px;
  }

  footer {
    height: auto;
  }

  footer div:nth-child(1) p {
    font-size: 12px;
  }

  footer div:nth-child(1) {
    max-width: 200px;
  }

  footer div:nth-child(2) {
    gap: 60px;
    width: auto;
  }

  footer ul {
    gap: 12px;
  }
}

@media (max-width: 882px) {

  .hero .light.light-orange {
    width: 60vw;
    height: 30vw;
  }

  .hero .light.light-yellow {
    width: 24vw;
    height: 10vw;
    top: 40vw;
  }

  .hero .light.light-blue {
    width: 41vw;
    height: 34vw;
    top: 77px;
    left: 50%;
  }

  header nav li:not(.connect, .login)  {
    display: none;
  }

  .burger {
    display: flex;
  }

  .logo {
    margin-left: 16px;
  }

  .logo img {
    width: 27px;
    height: 24px;
  }

  .logo span {
    color: var(--special-color);
    font-size: 22px;
    margin-left: 8px;
  }

  footer .logo {
    margin-left: 0;
  }

  
  .connect-btn {
    width: auto;
    height: auto;
    border-radius: 4px;
    padding: 6px 16px;
  } 

  .connect-btn span {
    font-weight: 700;
    font-size: 8px;
    line-height: 200%;
  }

  .connect-btn span:nth-child(2) {
    display: none;
  }


  .button {
    font-weight: 700;
    line-height: 200%;
    padding: 6px 16px;
    background: var(--special-color);
    border-radius: 4px;
    font-size: 8px;
  }

  .hero-card {
    height: 261px;
    width: 241px;
  } 

  .hero-card div {
    height: 70%;
  }

  .hero-wrap {
    padding: 100px 0 50px;
  }

  .hero h2 {
    margin-top: 34px;
  } 

  .collection .button, .subscribe .button, .hero .button {
    font-size: 14px;
  }

  .tocenomics-btn {
    font-size: 14px;
    border-radius: 4px;
    padding: 6px 16px;
    line-height: 200%;
  }
}

@media (max-width: 768px) {

  .container {
    padding: 0 40px;
  }

  header {
    padding: 7px 0 0;
  }

  .hero::before {
    width: 100%;
  }

  .hero-content-mobile {
    display: flex;
  }

  .hero-wrap {
    padding: 80px 0;
  }

  .functions {
    padding: 8vw 0 3vw;
  }

  .functions h4 {
    margin-top: 8vw;
  }

  .hero-content, .tocenomics-content, .tocenomics-btn, .functions-content, .collection-content, .collection .button {
    display: none;
  }

  .tocenomics-content-mobile, .tocenomics .light-blue, .functions-content-mobile, .functions .light-blue, .collection .light-orange, .collection-content-mobile, .collection-mobile-card::before,   .functions-items::before  {
    display: block;
  }

  .collection {
    padding: 14vw 0 2vw;
  }

  .contact img {
    bottom: 2vw;
  }

  .hero .light.light-yellow {
    width: 39vw;
    height: 27vw;
    top: 74vw;
    left: 28vw;
  }

  .hero .light.light-orange {
    width: 99vw;
    height: 45vw;
    top: 10vw;
    left: -27vw;
  }

  .beendexer .light.light-orange {
    width: 46vw;
    height: 61vw;
    right: 1%;
    top: 35vw;
  }

  .functions .light-blue {
    width: 46vw;
    height: 100vw;
    right: 53%;
    top: -60vw;
  }

  .collection .light-orange {
    width: 46vw;
    height: 75vw;
    right: 53%;
    top: -46vw; 
  }

  .contact {
    padding-top: 10vw;
    margin: 0 auto 10vw;
  }

  .subscribe .container {
    padding: 0;
  }

  .subscribe-card {
    border-radius: 0;
  }

  footer {
    padding: 40px 40px 20px;
    align-items: start;
    flex-direction: column;
  }

  footer div:nth-child(1) {
    max-width: 400px;
  }

  footer div:nth-child(2) {
    margin-top: 4vw;
    grid-auto-columns: 1fr 1fr 1fr;
  }

  footer li span {
    color: var(--special-color);
  }
}

@media (max-width: 539px) { 
  .container {
    padding: 0 20px;
  }

  .button:not(header .button) {
    line-height: 200%;
    padding: 10px 27px;
    border-radius: 11px;
    font-size: 14px;
  }

  .hero-wrap {
    padding: 60px 0;
  }

  .hero-content-mobile img {
    width: 255px;
    height: 255px;
  }

  .title {
    font-size: 3.6vw;
  } 

  .oval-button {
    width: 88px;
    height: 24px;
    padding: 0;
    justify-content: center;
  }

  .oval-button .pyramid {
    display: none;
  }

  .oval-button .text-field {
    font-size: 10px;
  }

  .teaser-picture {
    padding: 0;
    border: 0;
    background: none;
  }

  .beendexer h3 {
    font-size: 4vw;
  }  

  .beendexer-card {
    padding: 10px 24px;
    margin: 30px auto 0;
  }

  .beendexer-card p {
    text-transform: none;
    font-variant: normal;
  }

  .functions h4 {
    font-size: 4vw;
  } 

  .functions-item p {
    max-width: 324px;
    font-size: 14px;
    line-height: 140%;
  }

  .functions-items {
    margin: 28px auto 0;
    gap: 26px;
    grid-template: repeat(3, max-content) / 100%;
  }

  .functions-item {
    background: radial-gradient(98.05% 261.61% at 1.95% 3.59%, rgba(255, 255, 255, 0.4) 0%, rgba(255, 255, 255, 0) 100%);
    backdrop-filter: blur(40px);
    border-radius: 4px;
  }

  .functions-item .divider {
    margin-top: 18px;
    height: 3px;
  }

  .tocenomics {
    padding: 30px 0 20px;
  }

  .contact {
    margin: 0 auto 8vw;
    max-width: 80vw;
    max-height: 87vw;
  }

  .subscribe-card {
    padding: 40px 40px 120px;
  }

  .subscribe h3 {
    font-size: 4vw;
  }

  .subscribe p {
    font-size: 12px;
    max-width: 400px;
  } 

  .subscribe form {
    margin: 30px auto 0;
    grid-template-columns: 100%;
    grid-template-rows: 40px;
    height: auto;
    width: 100%;
  }

  .subscribe .button {
    margin: 0 auto;
    width: 120px;
    height: 57px;
  }

  .subscribe .light.light-orange {
    width: 73vw;
    height: 46vw;
    left: -4%;
    top: 73%;
  }   
  
  footer {
    margin-top: 0;
  } 

  footer::after {
    display: block;
  }
}

@media (max-width: 527px) { 
  .container {
    padding: 20px;
  }

  footer {
    padding: 40px 40px 100px;
  }

  footer div:nth-child(2) {
    margin-top: 8vw;
    grid-auto-columns: unset;
    grid-template-rows: max-content max-content max-content;
    grid-template-columns: unset;
    gap: 40px;
  }

  footer ul {
    display: grid;
    grid-template-rows: auto;
    gap: 14px;
  }

  footer div:nth-child(1) p, footer li span, footer li a {
    font-size: 16px;
  }

  footer div:nth-child(2) ul:nth-child(1) { order: 2}
  footer div:nth-child(2) ul:nth-child(2) { order: 3}
  footer div:nth-child(2) ul:nth-child(3) { order: 1}

  footer .light.light-yellow {
    width: 34vw;
    height: 111vw;
    right: 56vw;
    top: 64%;
  }

  footer .light.light-blue {
    display: block;
  }
} 

@media (max-width: 376px) {
  .container {
    padding: 20px;
  }

  footer {
    padding: 40px 20px 100px;
  }
}

@media (max-width: 374px) {
  header .logo span {
    display: none;
  }
}


</style>
