<template>
  <div class="foot-box">
    <div class="container">
      <div class="flex-box">
        <p>AvdSwap @ 2023, all rights reserved</p>
        <div class="icon-box">
          <font-awesome-icon :icon="['fab', 'facebook']" />
          <font-awesome-icon :icon="['fab', 'discord']" />
          <font-awesome-icon :icon="['fab', 'twitter']" />
          <font-awesome-icon :icon="['fab', 'telegram']" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.foot-box {
  background: #1A1A1A;
  height: 60px;
  .container {
    .flex-box {
        color: #fff;
        display: flex;
        justify-content: space-between;
        align-items: center;
        p {
            line-height: 60px;
            font-size: 20px;
        }
        .icon-box {
            padding-top: 5px;
            box-sizing: border-box;
            svg {
                margin-left: 20px;
                width:30px;
                height: 30px;
                cursor: pointer;
            }
        }
    }
  }
}
</style>