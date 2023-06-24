<template>
  <div class="tokenomics">
    <div class="container">
      <h3>Tokenomics</h3>
      <div class="flex-box">
        <div id="myChart" style="height: 400px; width: 60%"></div>
        <div class="title-content">
          <p>Make it truly decentralized, gradually</p>
          <p>burns TEAM tokens and</p>
          <p>drop management keys in the future</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  mounted() {
    this.drawChart();
  },
  methods: {
    drawChart() {
      // 基于准备好的dom，初始化echarts实例
      let myChart = this.$echarts.init(document.getElementById("myChart"));
      let options = {
        series: [
          {
            type: "pie",
            radius: ["35%", "70%"],
            color: ["#00A3FF", "#60D934", "#949192", "#F8BC00"],
            data: [
              {
                value: 70,
                name: "Community",
              },
              {
                value: 15,
                name: "Maketing",
              },
              {
                value: 5,
                name: "Airdop",
              },
              {
                value: 10,
                name: "Team",
              },
            ],
            label: {
              alignTo: "edge",
              formatter: "{name|{b}}\n{time|{c} %}",
              minMargin: 10,
              edgeDistance: 80,
              lineHeight: 26,
              rich: {
                time: {
                  fontSize: 18,
                  color: "#000",
                },
                name: {
                  fontSize: 18,
                  color: "#000",
                },
              },
            },
          },
        ],
      };
      myChart.setOption(options);
    },
  },
};
</script>

<style scoped lang="scss">
.tokenomics {
  background: #fff;
  .container {
    h3 {
      color: $base-color;
      font-size: $title-size;
      text-align: center;
      line-height: 32px;
      font-weight: 500;
      padding: 50px;
    }
    .flex-box {
      display: flex;
      justify-content: space-between;
      align-items: center;
      #myChart {
        flex: 1;
      }
      .title-content {
        text-align: right;
        margin-top: -50px;
        font-size: 20px;
        font-weight: 500;
      }
    }
  }
}
</style>