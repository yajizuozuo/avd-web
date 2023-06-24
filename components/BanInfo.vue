<template>
  <div class="banner-info">
    <div class="container">
      <!-- <div class="flex-box"> -->
      <!-- <img src="@/assets/images/threeBg.svg" /> -->
      <div class="content-box">
        <h3>What's AVDSWAP?</h3>
        <p>Avdwap is the first fully permissionless,</p>
        <p>oracle-less, non-liquidatable,</p>
        <p>fixed maturity lending & borrowing protocol.</p>
        <div class="tips-box">
          Avdswap aims to revolutionize money markets via.<br />
          its unique 3 variable constant product AMM
        </div>
        <!-- </div> -->
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.banner-info {
  background: $base-color;
  .container {
    background: url("~@/assets/images/threeBg.svg") left 120px bottom 0px no-repeat;
    background-size: contain;
  }
  .flex-box {
    display: flex;
    justify-content: space-between;
    img {
      height: 100%;
    }
  }
  .content-box {
    padding: 40px 0px 80px;
    text-align: right;
    color: #fff;
    h3 {
      color: #fff;
      margin-bottom: 40px;
      font-size: 42px;
    }
    & > P {
      font-size: 28px;
      line-height: 36px;
      font-weight: 500;
    }
    .tips-box {
      margin-top: 40px;
      padding-right: 18px;
      position: relative;
      display: inline-block;
      font-size: 16px;
      font-weight: 500;
      width: 500px;
      padding: 10px 12px;
      background: linear-gradient(to right,$base-color,#F7CCCE);
      &::after {
        content: "";
        position: absolute;
        width: 12px;
        background: #fff;
        height: 100%;
        right: 0;
        top: 0;
      }
    }
  }
}
</style>