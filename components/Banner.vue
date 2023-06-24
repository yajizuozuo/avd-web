<template>
    <div class="banner-box">
        <div class="container">
            <div class="content-box">
                <p>Fully decentralized</p>
                <p>AMM based money</p>
                <p>market protocol</p>
                <p class="tips">Powered by<span> OPTIMISM</span></p>
            </div>
            <!-- <div>
                <img src="@/assets/images/banner.svg" />
            </div> -->
        </div>
        
    </div>
</template>

<style scoped lang="scss">
.banner-box {
.container {
    background: url('~@/assets/images/banner.svg') right 160px bottom 0px no-repeat;
    // background-position-x: right 120px;
    background-size: contain;
    .content-box {
        padding-left: 40px;
        padding-top: 160px;
        padding-bottom: 60px;
        p {
            font-size: 48px;
            line-height: 56px;
            font-weight: 700;
            color: $base-color;
            &.tips {
                font-size: 20px;
                color: #000;
                margin-top: 20px;
                span{
                    color: $base-color;
                    font-style: italic;
                    padding-left: 12px;
                }
            }
        }
    }
}
}
</style>