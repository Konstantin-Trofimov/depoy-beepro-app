<template>
  <section class="functions">
    <div class="container">
      <div class="functions-wrap">
        <BlockHeading textTitle="Functions" />
        <div class="functions-content">
          <div class="functions-block">
            <img :src="beeLarge" alt="bee" />
          </div>
          <div class="functions-block">
            <div class="functions-cells">
              <div class="functions-cell">
                <span>1</span>
                <p>
                  Analysis of Blokchain
                  <br />
                  networks with
                  <br />
                  Smart Contracts
                </p>
              </div>
              <div class="functions-cell">
                <span>2</span>
                <p>
                  Calculation
                  <br />
                  of promising
                  <br />
                  projects
                </p>
              </div>
              <div class="functions-cell">
                <span>3</span>
                <p>Providing up-to-date information about cryptocurrencies</p>
              </div>
              <div class="functions-cell">
                <span>4</span>
                <p>
                  Compilation of ratings
                  <br />
                  of reliability of tokens
                </p>
              </div>
              <div class="functions-cell">
                <span>5</span>
                <p>
                  Checking available liquid currency pairs and finding new ones
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="functions-content-mobile">
          <div class="functions-mobile-wrap">
            <div 
              class="functions-mobile-cell functions-mobile-cell-top-right">
              <span>1</span>
              <p>Analysis of Blokchain networks with Smart Contracts</p>
            </div>
            <div 
              class="functions-mobile-cell functions-mobile-cell-top-left">
              <span>2</span>
              <p>Calculation of promising projects</p>
            </div>
            <div 
              class="functions-mobile-cell functions-mobile-cell-center">
              <span>3</span>
              <p>Providing up-to-date information about cryptocurrencies</p>
            </div>
            <div
              class="functions-mobile-cell functions-mobile-cell-bottom-right">
              <span>4</span>
              <p>Compilation of ratings of reliability of tokens</p>
            </div>
            <div
              class="functions-mobile-cell functions-mobile-cell-bottom-left">
              <span>5</span>
              <p>
                Checking available liquid currency pairs and finding new ones
              </p>
            </div>
          </div>
          <span class="light light-blue"></span>
        </div>
        <h4>Our functions</h4>
        <div class="functions-items">
          <div class="functions-item">
            <h5>TRADE</h5>
            <div class="divider"></div>
            <p>
              The BEEPRO exchange provides the opportunity to make anonymous
              transactions for the exchange of tokens located in the same
              blockchain network
            </p>
          </div>
          <div class="functions-item">
            <h5>STAKING</h5>
            <div class="divider"></div>
            <p>
              Allows you to receive passive income from cryptocurrencies running
              on the Proof-of Stake (PoS) algorithm and its varieties
            </p>
          </div>
          <div class="functions-item">
            <h5>POOLS</h5>
            <div class="divider"></div>
            <p>
              To become a liquidity provider (LP) you need to add two tokens of
              equal valueto your pool, thereby creating segregated market, after
              which you will be ableto profit from the commission on
              transactions made in the pool
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import BlockHeading from "./blocks/BlockHeading";
import beeLarge from "@/assets/images/functions/bee-large.png";
import сells from "@/assets/images/functions/сells.svg";

export default {
  components: {
    BlockHeading,
  },
  data: () => {
    return {
      beeLarge,
      сells,
    };
  },
};
</script>

<style>
.functions {
  padding: 100px 0 60px;
}

.functions-content {
  margin-top: 60px;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  height: 38vw;
}

.functions-block {
  position: relative;
}

.functions-content div:nth-child(1) img {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.functions-content div:nth-child(2) .functions-cells {
  position: absolute;
  width: 36vw;
  height: 36vw;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
}

.functions-content div:nth-child(2) .functions-cells::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  width: 100%;
  height: 100%;
  background: center / contain no-repeat
    url("../assets/images/functions/сells.svg");
}

.functions-cell {
  width: 30%;
  height: 30%;
  display: flex;
  align-items: center;
  justify-content: start;
  flex-direction: column;
  position: absolute;
  padding-top: 2%;
}

.functions-cell:nth-child(1) {
  top: 5.4%;
  left: 43.7%;
}
.functions-cell:nth-child(2) {
  top: 35.25%;
  left: 26.4%;
}
.functions-cell:nth-child(3) {
  top: 35.25%;
  left: 60.7%;
}
.functions-cell:nth-child(4) {
  top: 64.8%;
  left: 9.3%;
}
.functions-cell:nth-child(5) {
  top: 64.8%;
  left: 43.7%;
}

.functions-cell span {
  font-weight: 700;
  font-size: 1.8vw;
  color: var(--special-color);
}

.functions-cell p {
  margin-top: 18%;
  text-align: center;
  font-weight: 500;
  font-size: 0.6vw;
  line-height: 140%;
  text-align: center;
  font-variant: small-caps;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.functions-content-mobile {
  display: none;
  position: relative;
  width: 80vw;
  height: 80vw;
  margin: 6vw auto 0;
  z-index: 20;
}

.functions .light-blue {
  display: none;
}

.functions-mobile-wrap {
  width: 100%;
  height: 100%;
  position: relative;
}

.functions-mobile-wrap::before {
  content: "";
  position: absolute;
  width: 21vw;
  height: 21vw;
  left: 4%;
  top: 34%;
  background: center / contain no-repeat
    url("../assets/images/functions/bee.png");
  z-index: 30;
}

.functions-mobile-wrap::after{
  content: "";
  position: absolute;
  width: 27vw;
  height: 25vw;
  left: 52%;
  top: 40%;
  background: center / contain no-repeat
    url("../assets/images/functions/bee-neon.png");
  z-index: 30;
}

.functions-mobile-cell {
  position: absolute;
  transform: translate(-50%, -50%);
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-direction: column;
  padding: 6vw 6vw 9vw;
  z-index: 20;
}

.functions-mobile-cell span {
  font-weight: 700;
  font-size: 3.4vw;
  text-align: center;
  color: var(--special-color);
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25), 0px 4px 4px rgba(0, 0, 0, 0.25);
}

.functions-mobile-cell p {
  /* margin-top: 3.4vw; */
  font-weight: 500;
  font-size: 1.6vw;
  line-height: 130%;
  text-align: center;
  font-variant: small-caps;
  text-transform: uppercase;
}

.functions-mobile-cell::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  width: 100%;
  height: 100%;
  background: center / contain no-repeat
    url("../assets/images/functions/functions-cell.svg");
}

.functions-mobile-cell-center {
  width: 30vw;
  height: 30vw;
  top: 50%;
  left: 50%;
}

.functions-mobile-cell-top-left {
  width: 28vw;
  height: 28vw;
  top: 23%;
  left: 66%;
}

.functions-mobile-cell-top-right {
  width: 30.5vw;
  height: 30.5vw;
  top: 21%;
  left: 33%;
}

.functions-mobile-cell-bottom-left {
  width: 27.8vw;
  height: 27.8vw;
  top: 77%;
  left: 34%;
}

.functions-mobile-cell-bottom-right {
  width: 29.8vw;
  height: 29.8vw;
  top: 78%;
  left: 66%;
}

.functions h4 {
  margin-top: 210px;
  font-weight: 700;
  font-size: 36px;
  line-height: 44px;
  text-align: center;
  text-transform: uppercase;
}

.functions-items {
  margin: 60px auto 0;
  max-width: 1160px;
  height: 336px;
  display: grid;
  gap: 38px;
  grid-template: 336px / repeat(3, 1fr);
  position: relative;
}

.functions-items::before {
  content: "";
  position: absolute;
  width: 21vw;
  height: 21vw;
  left: -2%;
  top: -13vw;
  background: center / contain no-repeat
    url("../assets/images/functions/bee-white.png");
  z-index: 30;
  display: none;
}

.functions-item {
  background: rgba(161, 186, 209, 0.25);
  box-shadow: 0px 2px 23px rgba(0, 0, 0, 0.130507);
  border-radius: 12px;
  padding: 34px 36px 0;
  display: flex;
  align-items: center;
  justify-content: start;
  flex-direction: column;
  transition: all ease-out 1.9s;
}

.functions-item:nth-child(2) {
  background: linear-gradient(
    192.35deg,
    rgba(99, 130, 134, 0.8) 21.06%,
    rgba(255, 231, 107, 0.56) 72.79%,
    #ffe000 135.22%
  );
}

.functions-item h4 {
  font-weight: 700;
  font-size: 20px;
  line-height: 26px;
  text-align: center;
  letter-spacing: 0.07px;
}

.functions-item .divider {
  margin-top: 18px;
  width: 78px;
  height: 4px;
  background: #ffe001;
  border-radius: 2px;
}

.functions-item p {
  margin-top: 34px;
  font-weight: 400;
  font-size: 16px;
  line-height: 26px;
  text-align: center;
}
</style>