<template>
 <a href="#" class="logo">
   <img :src="logo" alt="logo"/>
   <span>BEEPRO</span>
 </a>
</template>

<script>
import logo from '@/assets/icons/logo.svg'

export default {
 data: () => {
   return {
     logo
   }
 },
}
</script>

<style>
.logo {
 display: flex;
 align-items: center;
}

.logo span {
 font-weight: 700;
 font-size: var(--fz-24);
 margin-left: 12px;
}

.logo img {
 width: 59px;
 height: 53px;
}

.logo span, .logo img {
 position: relative;
 z-index: 20;
}
</style>