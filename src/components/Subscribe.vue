<template>
 <section class="subscribe">
   <div class="container">
     <div class="subscribe-wrap">
       <div class="subscribe-card">
        <h3>Stay in the Commynity</h3>
        <p>It should be noted that the further development of various 
        forms of activity is a qualitatively new stage in the analisis 
        of existing patterns of behavior</p>
        <form action="#">
         <input placeholder="Your Email" type="text">
         <Button text="Subscribe"/>
        </form>
       </div>
       <span class="light light-orange"></span>
       <span class="light light-yellow"></span>
     </div>
   </div>
 </section>
</template>

<script>
import Button from './buttons/Button'

export default {
 components: {
  Button
 }, 
 data: () => {
   return {
    
   };
 },
};
</script>

<style>
.subscribe {
 padding: 160px 0 100px;
}

.subscribe-card {
 max-width: 1232px;
 margin: 0 auto;
 padding: 70px 0;
 background: radial-gradient(98.05% 261.61% at 1.95% 3.59%, rgba(255, 255, 255, 0.4) 0%, rgba(255, 255, 255, 0) 100%);
 backdrop-filter: blur(40px);
 border-radius: 8px;
 display: flex;
 flex-direction: column;
 align-items: center;
 justify-content: start;
 position: relative;
 z-index: 20;
}

.subscribe h3 {
 font-weight: 700;
 font-size: var(--fz-48);
 line-height: 130%;
 text-align: center;
 text-transform: capitalize;
 font-feature-settings: 'pnum' on, 'lnum' on;
 max-width: 537px;
}

.subscribe p {
 margin-top: 32px;
 font-weight: 500;
 line-height: 160%;
 max-width: 502px;
 text-align: center;
}

.subscribe form {
 margin-top: 46px;
 max-width: 676px;
 height: 56px;
 display: grid;
 grid-template-columns: minmax(300px, 513px) auto;
 gap: 16px;
}

.subscribe input {
 height: 100%;
 background: var(--color-white);
 border-radius: 8px;
 border: none;
 font-weight: 500;
 line-height: 160%;
 color: var(--text-input-color);
 padding: 15px 16px;
 position: relative;
 z-index: 20;
}

.subscribe .light.light-orange {
 width: 16vw;
 height: 10vw;
 left: 16%;
 top: 50%;
 transform: translateY(-50%);
 filter: blur(160px);
}

.subscribe .light.light-yellow {
 width: 34vw;
 height: 6vw;
 right: 20%;
 top: 50%;
 transform: translateY(-50%);
}


</style>