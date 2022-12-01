<template>
  <section class="teaser">
    <div class="container">
      <div class="teaser-wrap">
        <BlockHeading textTitle="Teaser" />
        <div class="teaser-picture">
          <img :src="teaserImg" alt="picture" />
        </div>
        <span class="light light-blue"></span>
        <span class="light light-orange"></span>
        <span class="light light-yellow"></span>
      </div>
    </div>
  </section>
</template>

<script>
import BlockHeading from "./blocks/BlockHeading";
import teaserImg from "@/assets/images/teaser/teaser-img.png";

export default {
  components: {
    BlockHeading,
  },
  data: () => {
    return {
      teaserImg,
    };
  },
};
</script>

<style>
.teaser {
 padding: 260px 0 100px;
}

.teaser-picture {
  margin: 60px auto 0;
  position: relative;
  max-width: 115%;
  max-width: 1356px;
  background: linear-gradient(
    149deg,
    rgba(255, 255, 255, 0) 0%,
    rgba(110, 121, 113, 1) 100%
  );
  padding: 18px 21px 18px 19px;
  border: 1px solid #979797;
  z-index: 20;
}

.teaser-picture img {
  object-fit: contain;
  width: 100%;
  height: auto;
  z-index: 20;
}

.teaser .light.light-blue {
 width: 24vw;
 height: 22vw;
 top: 40%;
 right: 0px;
}

.teaser .light.light-orange {
 width: 22vw;
 height: 22vw;
 left: 42vw;
 top: 10vw;
}

.teaser .light.light-yellow {
 width: 24vw;
 height: 8vw;
 right: 20%;
 bottom: 5%;
}


</style>