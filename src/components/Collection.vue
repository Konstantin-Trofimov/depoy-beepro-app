<template>
  <section class="collection">
    <div class="container">
      <div class="collection-wrap">
        <BlockHeading textTitle="NFT Collection" />
        <div class="collection-content">
          <div class="collection-card">
            <div class="collection-card-preview"></div>
            <div class="collection-card-descr">
              <div class="collection-autor">
                <div class="collection-autor-avatar"></div>
                <span class="collection-autor-name">Yerikho Christian</span>
              </div>
              <h5 class="collection-name">Collection #1</h5>
              <div class="collection-data">
                <div>
                  <span>Current Bid</span>
                  <span>Auction ending in</span>
                </div>
                <div>
                  <p>0.4435 ETH</p>
                  <p>10:12:32</p>
                </div>
              </div>
            </div>
          </div>
          <div class="collection-card">
            <div class="collection-card-preview"></div>
            <div class="collection-card-descr">
              <div class="collection-autor">
                <div class="collection-autor-avatar"></div>
                <span class="collection-autor-name">Yerikho Christian</span>
              </div>
              <h5 class="collection-name">Collection #1</h5>
              <div class="collection-data">
                <div>
                  <span>Current Bid</span>
                  <span>Auction ending in</span>
                </div>
                <div>
                  <p>0.4435 ETH</p>
                  <p>10:12:32</p>
                </div>
              </div>
            </div>
          </div>
          <div class="collection-card">
            <div class="collection-card-preview"></div>
            <div class="collection-card-descr">
              <div class="collection-autor">
                <div class="collection-autor-avatar"></div>
                <span class="collection-autor-name">Yerikho Christian</span>
              </div>
              <h5 class="collection-name">Collection #1</h5>
              <div class="collection-data">
                <div>
                  <span>Current Bid</span>
                  <span>Auction ending in</span>
                </div>
                <div>
                  <p>0.4435 ETH</p>
                  <p>10:12:32</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="collection-content-mobile">
          <div class="collection-mobile-card">
            <div class="collection-card-preview"></div>
            <div class="collection-card-descr">
              <div class="collection-autor">
                <div class="collection-autor-avatar"></div>
                <span class="collection-autor-name">Yerikho Christian</span>
              </div>
              <h5 class="collection-name">Collection #1</h5>
              <div class="collection-data">
                <div>
                  <span>Current Bid</span>
                  <span>Auction ending in</span>
                </div>
                <div>
                  <p>0.4435 ETH</p>
                  <p>10:12:32</p>
                </div>
              </div>
            </div>
          </div>
          <div class="collection-dots">
            <span></span>
            <span></span>
            <span></span>
          </div>
          <div class="collection-arrow"></div>
          <span class="light light-orange"></span>
        </div>
        <Button text="Buy and play" />
      </div>
    </div>
  </section>
</template>

<script>
import BlockHeading from "./blocks/BlockHeading";
import Button from "./buttons/Button";

export default {
  components: {
    BlockHeading,
    Button,
  },
  data: () => {
    return {};
  },
};
</script>

<style>
.collection {
  padding: 120px 0 60px;
}

.collection-wrap {
  text-align: center;
}

.collection-content {
  text-align: center;
  margin: 80px auto 82px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.collection-card {
  position: relative;
  height: 660px;
  width: 442px;
}

.collection-card-preview {
  background: center / contain no-repeat
    url("../assets/images/collection/collection-preview-bg.svg");
  width: 100%;
  height: 423px;
}

.collection-card-descr {
  background: center / contain no-repeat
    url("../assets/images/collection/collection-descr-bg.svg");
  position: absolute;
  top: 343px;
  width: 100%;
  height: 319px;
  padding: 106px 50px 0;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: start;
}

.collection-autor {
  display: flex;
  align-items: center;
  justify-content: center;
}

.collection-autor span {
  margin-left: 8px;
  font-weight: 500;
  font-size: var(--fz-14);
}

.collection-autor-avatar {
  background: var(--grey-color);
  width: 32px;
  height: 32px;
  border-radius: 100%;
}

.collection-name {
  font-weight: 700;
  font-size: var(--fz-32);
  text-transform: capitalize;
  font-feature-settings: "pnum" on, "lnum" on;
  color: var(--special-color);
  margin-top: 16px;
}

.collection-data {
  width: 100%;
  margin-top: 24px;
}

.collection-data div {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.collection-data div:nth-child(2) {
  margin-top: 10px;
}

.collection-data span,
.collection-data p {
  text-align: left;
}

.collection-data span {
  font-weight: 500;
  font-size: var(--fz-14);
}

.collection-data p {
  font-weight: 700;
  font-size: var(--fz-24);
  text-transform: capitalize;
  font-feature-settings: "pnum" on, "lnum" on;
}

.collection-content-mobile {
  display: none;
  width: 80vw;
  height: 80vw;
  position: relative;
  margin: 56px auto 0;
}

.collection-mobile-card {
  position: relative;
  width: 100%;
  height: 100%;
  z-index: 30;
}

.collection-content-mobile .collection-card-preview {
  position: absolute;
  left: 50%;
  transform: translate(-50%, -50%);
  top: 25vw;
  height: 44vw;
  width: 40vw;
}

.collection-content-mobile .collection-card-descr {
  position: absolute;
  left: 50%;
  transform: translate(-50%, -50%);
  top: 55vw;
  height: 40vw;
  width: 40vw;
  padding: 16vw 3vw 0;
}

.collection-content-mobile .collection-autor-avatar {
  width: 4vw;
  height: 4vw;
}

.collection-content-mobile .collection-autor span {
  font-size: 2vw;
}

.collection-content-mobile .collection-name {
  font-size: 3vw;
  margin-top: 2vw;
}

.collection-content-mobile .collection-data {
  margin-top: 2.6vw;
}

.collection-content-mobile .collection-data span {
  font-size: 2vw;
}

.collection-content-mobile .collection-data p {
  font-size: 2.4vw;
}

.collection-dots {
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 2vw;
}

.collection-dots span {
  margin-left: .2vw;
  margin-right: .2vw;
  background: var(--second-grey-color);
  border: .5vw solid var(--black-color);
  border-radius: 100%;
  width: 3vw;
  height: 3vw;
}

.collection-arrow {
  position: absolute;
  top: 50%;
  right: 0;
  width: 5vw;
  height: 6vw;
  background: center / contain no-repeat
    url("../assets/images/collection/arrow.svg");
  z-index: 50;

}

.collection-mobile-card::before {
  content: "";
  position: absolute;
  width: 26vw;
  height: 25vw;
  left: 9%;
  top: -9%;
  background: center / contain no-repeat
    url("../assets/images/collection/bee-in-hat.png");
  z-index: 30;
  display: none;
}


.collection .light-orange {
  display: none;
}

</style>