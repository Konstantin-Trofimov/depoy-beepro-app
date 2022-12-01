<template>
 <section class="roadmap">
  <div class="container">
   <div class="roadmap-wrap">
    <BlockHeading textTitle="Roadmap" />
    <div class="roadmap-content">
     <img :src="roadmap" alt="">
    </div>
   </div>
  </div>
 </section>
</template>

<script>
import BlockHeading from './blocks/BlockHeading'
import roadmap from '@/assets/images/roadmap/roadmap.svg'


export default {
  components: {
    BlockHeading,
  },
  data: () => {
    return {
     roadmap
    };
  },
};
</script>

<style>
 .roadmap {
  display: none;
  padding: 80px 0 20px;
 }

 .roadmap-content {
  margin: 75px auto 0;
  text-align: center;
 }
</style>