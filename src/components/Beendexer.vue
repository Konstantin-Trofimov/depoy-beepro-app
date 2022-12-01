<template>
 <section class="beendexer">
  <div class="container">
   <div class="beendexer-wrap">
    <h3>beendexer</h3>
    <div class="beendexer-card">
     <p>
      Beendexer technology allows you to find the best
      crypto projects on the best on the market like
      a bee that selects only the sweetest nectar in a flower field
     </p>
    </div>
    <span class="light light-orange"></span>
    <span class="light light-yellow"></span>
   </div>
  </div>
 </section>
</template>



<style>
.beendexer {
 padding: 150px 0 100px;
}

.beendexer h3, .beendexer-card, .beendexer-card p {
 position: relative;
 z-index: 30;
}

.beendexer h3 {
 font-weight: 700;
 font-size: var(--fz-55);
 line-height: 160%;
 text-align: center;
 text-transform: uppercase;
 font-feature-settings: 'pnum' on, 'lnum' on;
}

.beendexer-card {
 margin: 60px auto 0;
 max-width: 1258px;
 padding: 100px 120px;
 background: radial-gradient(98.05% 261.61% at 1.95% 100.59%, rgba(255, 255, 255, 0) 0%, rgba(255, 255, 255, 0.4) 100%);
 backdrop-filter: blur(40px);
 border-radius: 8px;
 display: flex;
 align-items: center;
 justify-content: center;
}

.beendexer-card p{
 max-width: 800px;
 font-weight: 500;
 font-size: var(--fz-22);;
 line-height: 180%;
 text-align: center;
 font-variant: small-caps;
 text-transform: uppercase;
 letter-spacing: 1px;
}

.beendexer .light.light-orange {
 width: 16vw;
 height: 10vw;
 right: 20%;
 top: 10vw;
 filter: blur(160px);
}

.beendexer .light.light-yellow {
 width: 34vw;
 height: 6vw;
 left: 16%;
 top: 67%;
 transform: translateY(-50%);
}
</style>