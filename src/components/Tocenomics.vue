<template>
  <section class="tocenomics">
    <div class="container">
      <div class="tocenomics-wrap">
        <BlockHeading textTitle="Tocenomics" />
        <div class="tocenomics-content">
          <img class="tocenomics-diagram" :src="tocenomics" alt="tocenomics" />
        </div>
        <button class="tocenomics-btn">BUY TOKEN</button>
        <div class="tocenomics-cell tocenomics-master-cell tocenomics-content-mobile">
          <!-- <img :src="tocenomicsBg" alt=""/> -->
          <div class="tocenomics-cell tocenomics-cell-sub tocenomics-center">
            <div>
              <span>8%</span>
              <span>SEED ROUND</span>
            </div>
          </div>
          <div class="tocenomics-cell tocenomics-cell-sub tocenomics-top-right">
            <div>
              <span>5%</span>
              <span>PUBLIC ROUND</span>
            </div>
          </div>
          <div class="tocenomics-cell tocenomics-cell-sub tocenomics-right">
            <div>
              <span>15%</span>
              <span>private round</span>
            </div>
          </div>
          <div
            class="tocenomics-cell tocenomics-cell-sub tocenomics-bottom-right"
          >
            <div>
              <span>20%</span>
              <span>Treasury</span>
            </div>
          </div>
          <div
            class="tocenomics-cell tocenomics-cell-sub tocenomics-bottom-left"
          >
            <div>
              <span>20%</span>
              <span>EVENTS</span>
            </div>
          </div>
          <div class="tocenomics-cell tocenomics-cell-sub tocenomics-left">
            <div>
              <span>12%</span>
              <span>Team</span>
            </div>
          </div>
          <div class="tocenomics-cell tocenomics-cell-sub tocenomics-top-left">
            <div>
              <span>20%</span>
              <span>Liquidity pool</span>
            </div>
          </div>
        </div>
        <div class="tocenomics-cell tocenomics-content-mobile tocenomics-info">
          <div class="tocenomics-info-items">
            <div>
              <span>Liquidity pool</span>
              <p>Volume: 200.000.000, vesting 30% TGE+17,5% over 4 months)</p>
            </div>
            <div>
              <span>Events</span>
              <p>200.000.000, vesting 5 % over 20 months</p>
            </div>
            <div>
              <span>TREASURy</span>
              <p>Volume:200.000.000, vesting: 8.3% over 12 months</p>
            </div>
            <div>
              <span>Team</span>
              <p>
                Volume:120.000.000, vesting:1 month clif+10% over 10 months)
              </p>
            </div>
            <div>
              <span>seed round</span>
              <p>
                Keeps price at 0.02$(raised 1.600.000$ , volume: 80.000.000,
                vesting:5% TGE + 11,875 over 8 months
              </p>
            </div>
            <div>
              <span>Public round</span>
              <p>
                Keeps price at 0.05$(raised 2.500.000$, volume: 50.000.000,
                vesting:20% TGE + 20% over 4 months)
              </p>
            </div>
            <div>
              <span>PRIVATE ROUND</span>
              <p>
                Keeps price at 0.03$(raised 4.500.000$, volume: 150.000.000,
                vesting:10% TGE + 15% over 6 months)
              </p>
            </div>
            <div class="tocenomics-info-img"></div>
          </div>
        </div>
        <span class="light light-blue"></span>
      </div>
    </div>
  </section>
</template>

<script>
import BlockHeading from "./blocks/BlockHeading";
import tocenomics from "@/assets/images/tocenomics/tocenomics.svg";
// import tocenomicsBg from '@/assets/images/tocenomics/tocenomics-bg.svg'

export default {
  components: {
    BlockHeading,
  },
  data: () => {
    return {
      tocenomics,
      // tocenomicsBg
    };
  },
};
</script>

<style>
.tocenomics {
  padding: 80px 0 20px;
}

.tocenomics-content {
  margin: 56px 0 auto;
  position: relative;
  text-align: center;
}

.tocenomics-content .tocenomics-diagram {
  width: 100%;
  height: auto;
}

.tocenomics-btn {
  display: block;
  margin: 20px auto 0;
  padding: 15px 51px;
  background: linear-gradient(13.34deg, #fe5500 16.35%, #fe8900 85.45%);
  box-shadow: inset 2.39333px -2.39333px 2.39333px rgba(213, 93, 0, 0.4),
    inset -2.39333px 2.39333px 2.39333px rgba(255, 255, 255, 0.4);
  backdrop-filter: blur(2.154px);
  font-weight: 700;
  font-size: 30.1613px;
  line-height: 39px;
  letter-spacing: 0.100538px;
  color: var(--black-color);
  cursor: pointer;
  border-radius: 6px;
  text-transform: uppercase;
  border: none;
}

.tocenomics-content-mobile {
  display: none;
}

.tocenomics-master-cell {
  position: relative;
  margin-top: 7vw;
  width: 80vw;
  height: 80vw;
  margin: 0 auto;
}

/* .tocenomics-master-cell img {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  width: 100%;
  height: 100%;
} */

.tocenomics-cell::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  width: 100%;
  height: 100%;
}

.tocenomics-cell-sub {
  position: absolute;
  transform: translate(-50%, -50%);
  display: flex;
  justify-content: center;
  align-items: center;
}

.tocenomics-cell-sub div {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: relative;
  z-index: 20;
  width: 100%;
  height: 100%;
  text-align: center;
}

.tocenomics-cell-sub span {
  width: 60%;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  font-weight: 700;
  text-transform: uppercase;
  font-size: 2vw;
}

.tocenomics-center div {
  justify-content: flex-start;
  margin-top: 55%;
}

.tocenomics-cell-sub span:nth-child(2) {
  margin-top: 3%;
}

.tocenomics-content-mobile::before {
  background: center / contain no-repeat
    url("../assets/images/tocenomics/tocenomics-bg.svg");
}

.tocenomics-center {
  top: 50%;
  left: 50%;
  width: 28vw;
  height: 28vw;
}

.tocenomics-center::before {
  background: center / contain no-repeat
    url("../assets/images/tocenomics/tocenomics-cell-center.svg");
}

.tocenomics-top-right {
  top: 29%;
  left: 64%;
  width: 16vw;
  height: 16vw;
}

.tocenomics-top-right::before {
  background: center / contain no-repeat
    url("../assets/images/tocenomics/small-dark-cell.svg");
}

.tocenomics-right {
  top: 50%;
  left: 79%;
  width: 22vw;
  height: 22vw;
}

.tocenomics-right::before {
  background: center / contain no-repeat
    url("../assets/images/tocenomics/medium-orange-cell.svg");
}

.tocenomics-bottom-right {
  top: 75%;
  left: 65%;
  width: 24vw;
  height: 24vw;
}

.tocenomics-bottom-right::before {
  background: center / contain no-repeat
    url("../assets/images/tocenomics/large-yellow-celll.svg");
}

.tocenomics-bottom-left {
  top: 76%;
  left: 34%;
  width: 26vw;
  height: 26vw;
}

.tocenomics-bottom-left::before {
  background: center / contain no-repeat
    url("../assets/images/tocenomics/large-orange-cell.svg");
}

.tocenomics-left {
  top: 49%;
  left: 24%;
  width: 18vw;
  height: 18vw;
}

.tocenomics-left::before {
  background: center / contain no-repeat
    url("../assets/images/tocenomics/medium-dark-cell.svg");
}

.tocenomics-top-left {
  top: 22%;
  left: 34%;
  width: 26vw;
  height: 26vw;
}

.tocenomics-top-left::before {
  background: center / contain no-repeat
    url("../assets/images/tocenomics/large-orange-cell.svg");
}

.tocenomics-info {
  top: -4vw;
  width: 70vw;
  position: relative;
  margin: 0 auto;
  top: -22vw;
  left: -0.5vw;
  height: 107vw;
  padding: 27vw 8vw 7vw;
  z-index: 20;
  margin-bottom: -22vw;
}

.tocenomics-info::before {
  background: center / contain no-repeat
    url("../assets/images/tocenomics/tocenomics-info-bg.svg");
}

.tocenomics-info-items {
  width: 100%;
  height: 100%;
  display: grid;
  grid-template-columns: 50% 50%;
  grid-template-rows: repeat(3, 22%);
  column-gap: 1vw;
  row-gap: 2vw;
}

.tocenomics-info-items div {
  padding-left: 6vw;
  position: relative;
}

.tocenomics-info-items div:not(.tocenomics-info-img)::before {
  content: "";
  position: absolute;
  width: 5vw;
  height: 5vw;
  left: 0;
  top: -0.6vw;
  background: center / contain no-repeat
    url("../assets/images/tocenomics/tocenomics-mark.svg");
}

.tocenomics-info-items div span {
  font-weight: 700;
  font-size: 2vw;
  text-transform: uppercase;
  font-feature-settings: "pnum" on, "lnum" on;
  text-shadow: 0px 20.5px 20.5px rgba(0, 0, 0, 0.25);
}

.tocenomics-info-items div p {
  margin-top: 1vw;
  font-weight: 400;
  font-size: 1.4vw;
  line-height: 180%;
  text-transform: uppercase;
  font-feature-settings: "pnum" on, "lnum" on;
  color: #ffffff;
  text-shadow: 0px 3.91667px 3.91667px rgba(0, 0, 0, 0.25);
}

.tocenomics-info-img::before {
  content: "";
  position: absolute;
  width: 30vw;
  height: 30vw;
  left: 10%;
  background: center / contain no-repeat
    url("../assets/images/tocenomics/tocenomics-bee.png");
}

.tocenomics .light-blue {
  display: none;
  width: 60vw;
  height: 91vw;
  left: 31%;
  bottom: 13%;
  opacity: 1;
}
</style>