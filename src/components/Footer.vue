<template>
 <footer>
   <div>
    <BlockLogo/>
    <p>A marketplace that sells various types of work by professional designers and is paid with NFT tokens.</p>
   </div>
   <div>
    <ul>
     <li>
      <span>About Us</span>
     </li>
     <li>
      <a>About Us</a>
     </li>
     <li>
      <a>Our Services</a>
     </li>
     <li>
      <a>How It Works</a>
     </li>
     <li>
      <a>Become a Partner</a>
     </li>
    </ul>

    <ul>
     <li>
      <span>Community</span>
     </li>
     <li>
      <a>Token</a>
     </li>
     <li>
      <a>Discussion</a>
     </li>
     <li>
      <a>Voting</a>
     </li>
     <li>
      <a>Blog</a>
     </li>
     <li>
      <a>Help Center</a>
     </li>
    </ul>

    <ul>
     <li>
      <span>Social Media</span>
     </li>
     <li>
      <a>Instagram</a>
     </li>
     <li>
      <a>Facebook</a>
     </li>
     <li>
      <a>Telegram</a>
     </li>
     <li>
      <a>Instagram</a>
     </li>
     <li>
      <a>Discord</a>
     </li>
     <li>
      <a>Raddit</a>
     </li>
    </ul>
   </div>
   <span class="light light-orange"></span>
   <span class="light light-yellow"></span>
   <span class="light light-blue"></span>
 </footer>
</template>


<script>
import BlockLogo from './blocks/BlockLogo'

export default {
  components: {
   BlockLogo
  }, 
}
</script>

<style>
footer {
 position: relative;
 margin-top: 100px;
 width: 100%;
 height: 398px;
 padding: 50px 300px 0 100px;
 background: radial-gradient(98.05% 261.61% at 1.95% 3.59%, rgba(255, 255, 255, 0.4) 0%, rgba(255, 255, 255, 0) 100%);
 backdrop-filter: blur(40px);
 display: flex;
 align-items: center;
 justify-content: space-between;
}

footer::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 2px;
  background: rgba(255, 255, 255, 0.4);
  z-index: 50;
  display: none;
}

footer::after {
  content: "";
  position: absolute;
  width: 36vw;
  height: 36vw;
  left: 57vw;
  top: -25vw;
  background: center / contain no-repeat url("../assets/images/bee-footer.png");
  z-index: 80;
  display: none;
}

footer div:nth-child(1) {
 max-width: 279px;
}

footer div:nth-child(1) p {
 margin-top: 24px;
 font-weight: 500;
 line-height: 160%;
}

footer div:nth-child(2) {
 width: 557px;
 display: grid;
 grid-template-columns: max-content max-content max-content;
 gap: 107px;
}

footer ul {
 display: grid;
 grid-template-rows: repeat(6, 24px);
 gap: 16px;
}

footer li span {
 font-weight: 700;
 line-height: 200%;
}

footer li a {
 font-weight: 400;
 font-size: var(--fz-14);
 line-height: 170%;
}

footer, footer li a, footer li span, footer div:nth-child(1) p {
 position: relative;
 z-index: 20;
}


footer .light.light-orange {
 width: 16vw;
 height: 10vw;
 left: 16%;
 top: 50%;
 transform: translateY(-50%);
 filter: blur(160px);
}

footer .light.light-yellow {
 width: 34vw;
 height: 6vw;
 right: 20%;
 top: 50%;
 transform: translateY(-50%);
}

footer .light.light-blue {
  width: 57vw;
  height: 97vw;
  bottom: 3vw;
  left: 25vw;
  display: none;
  opacity: 1;
}

</style>