

<template>
  <header>
   <div class="container">
    <div class="burger">
      <span></span>
      <span></span>
      <span></span>
    </div>
    <div class="header-wrap">
     <BlockLogo/>
     <nav>
      <ul>
       <li>
        <a href="">About</a>
       </li>
       <li>
        <a href="">Products</a>
       </li>
       <li>
        <a href="">Trades</a>
       </li>
       <li>
        <a href="">Earn</a>
        <img class="dropdown-arrow" :src="dropdownArrow"/>
       </li>
       <li>
        <span>Documents</span>
        <img class="dropdown-arrow" :src="dropdownArrow"/>
       </li>
       <!-- <li class="lang">
        <span>Eng</span>
        <img class="dropdown-arrow" :src="dropdownArrow"/>
       </li> -->
       <li class="connect">
        <button class="connect-btn"><span>Connect</span><span> Wallet</span></button>
       </li>
       <li class="login">
        <Button/>
       </li>
      </ul>
     </nav>
    </div>
   </div>   
  </header>
</template>

<script>
import Button from './buttons/Button'
import BlockLogo from './blocks/BlockLogo'
import dropdownArrow from '@/assets/icons/dropdown-arrow.svg'


export default {
  components: {
   Button,
   BlockLogo
  }, 
  data: () => {
    return {
      dropdownArrow,
    }
  },
}
</script>

<style>
header {
 position: absolute;
 top: 0;
 z-index: 40;
 width: 100%;
 padding: 32px 0 0;
} 

header .container {
  display: flex;
  align-items: center;
}

header .header-wrap {
 width: 100%;
 display: flex;
 justify-content: space-between;
 align-items: center;
}

header nav ul {
 display: flex;
 align-items: center;
 justify-content: center;
}

header nav li {
 padding: 0 20px;
 cursor: pointer;
}

header nav li span, nav li a {
 font-weight: 500;
}

header nav li .dropdown-arrow {
 margin-left: 8px;
}

.connect {
 padding: 0 0 0 8vw;
}

.connect-btn {
 background: rgba(255, 255, 255, 0.1);
 box-shadow: inset 0.924667px -0.924667px 0.924667px rgba(214, 214, 214, 0.4), inset -0.924667px 0.924667px 0.924667px rgba(255, 255, 255, 0.4);
 backdrop-filter: blur(8.36823px);
 width: 102px;
 height: 19px;
 border-radius: 6.65px;
 border: none;
 cursor: pointer;
 display: flex;
 align-items: center;
 justify-content: center;
} 

.connect-btn span  {
  font-weight: 400;
  font-size: 9px;
  text-transform: uppercase;
}

.connect-btn span:nth-child(2)  {
  margin-left: 3px;
}

.login {
 padding: 0 0 0 30px;
}

.burger {
  width: 16px;
  height: 12px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
  display: none;
}

.burger span{
  height: 2px;
  background: var(--color-white);
}

.burger span:nth-child(1) {width: 16px;}
.burger span:nth-child(2) {width: 12px;}
.burger span:nth-child(3) {width: 6px;}

</style>