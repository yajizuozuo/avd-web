<template>
  <div class="head-box">
    <div class="container">
      <div class="flex-box">
        <div class="logo-box">
          <img src="@/assets/images/logo.svg" />
        </div>

        <div class="menu-box">
          <div class="">Network<a-icon type="caret-down" /></div>
          <div class="">Products<a-icon type="caret-down" /></div>
          <div class="">Airdrops</div>
          <div class="">Whiepaper</div>
        </div>
        <div class="btn-box">
          <a-button type="danger">Connect</a-button>
        </div>
      </div>
    </div>
    <!-- <div class="container is-fluid">
        <div class="navbar is-spaced is-success"><img src="@/assets/images/logo.svg"></div>
        <div class="">
            <a-menu v-model="current" mode="horizontal">
                <a-menu-item key="mail">  Network<a-icon type="caret-down" /></a-menu-item>
                <a-menu-item key="mail">  Products<a-icon type="caret-down" /></a-menu-item>
                <a-menu-item key="mail">  Airdrops</a-menu-item>
                <a-menu-item key="mail">  Whiepaper</a-menu-item>
            </a-menu>
        </div>
        <div class="">
            <a-button type="danger">Connect</a-button>
        </div>
    </div> -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      current: [],
    };
  },
};
</script>
<style scoped lang="scss">
.head-box {
    height: 80px;
    line-height: 80px;
    .container {
        .flex-box {
            display: flex;
            justify-content: space-between;
            align-items: center;
            .logo-box {
                img {
                    height: 32px;
                }
            }
            .menu-box {
                flex: 1;
                display: flex;
                justify-content: space-around;
                align-items: center;
                color: $base-color;
                div {
                    cursor: pointer;
                    font-size: 20px;
                    font-weight: 500;
                    i {
                        margin-left: 6px;
                    }
                }
            }
            .btn-box {
                .ant-btn-danger {
                    background: $base-color;
                    border-color: $base-color;
                }
            }
        }
    }
}
</style>