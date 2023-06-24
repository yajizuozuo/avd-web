<template>
  <div class="road-map">
    <div class="container">
      <h3>Our Roadmap</h3>
      <div style="margin-top: 20px;">
        <a-row type="flex" justify="space-between" :gutter="[40, 40]">
          <a-col :span="8">
            <div class="content-box">
              <p>Phase 1</p>
              <div>
                <p>Token creation</p>
                <p>Launch on uni DEX</p>
                <p>Digital identity creation</p>
                <p>White paper creation</p>
                <p>Community building</p>
                <p>Community sensitization</p>
              </div>
            </div>
          </a-col>
          <a-col :span="8">
            <div class="content-box">
              <p>Phase 2</p>
              <div>
                <p>Website creation</p>
                <p>Twitter spaces with prominent</p>
                <p>KOLs</p>
                <p>Community education</p>
                <p>campaign for velodrome DEX</p>
                <p>Whitelisting for bribes and</p>
                <p>farming on velodrome DEX</p>
              </div>
            </div>
          </a-col>
          <a-col :span="8">
            <div class="content-box">
              <p>Phase 3</p>
              <div>
                <p>DAO creation</p>
                <p>Launch of governance</p>
                <p>mechanism</p>
                <p>Testnet Launch</p>
              </div>
            </div>
          </a-col>
        </a-row>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.road-map {
  background: linear-gradient(#feafbc, #ffc2a0);
  padding-bottom: 50px;
  h3 {
    color: $base-color;
    font-size: $title-size;
    text-align: center;
    line-height: 32px;
    font-weight: 500;
    padding: 20px 30px;
  }
  .content-box {
    border: 1px dashed $base-color;
    padding: 40px 30px;
    height: 350px;
    background: linear-gradient(#FFF, #FFC2A4);
    & > p {
        font-size: 24px;
        font-weight: 500;
        color: $base-color;
        margin-bottom: 18px;
    }
    & > div {
        font-size: 20px;
        font-weight: 500;
    }
  }
}
</style>