<template>
  <div>
    <div :class="{ footer: big, small: !big }">
      <div class="right">
        <span v-if="big"
          >COPYRIGHT©2023，www.icc.ah.cn , All rights
          reserved.<br />版权所有 © 全球发明大会中国区安徽赛区 未经许可 严禁复制
          皖ICP备2022015871号-2</span
        >
        <span v-if="!big"
          >《版权所有》COPYRIGHT©2023，www.icc.ah.cn<br /> , All rights
          reserved.<br />版权所有 © 全球发明大会中国区安徽赛区<br />
          皖ICP备2022015871号-2</span
        >
      </div>
      <div class="left">
        <div class="img" v-if="big">
          <img src="./image/logo2.png" alt="" class="img1" />
          <img src="./image/logo3.png" alt="" class="img2" />
        </div>
        <div class="ma">
          <div class="ma1">
            <img src="./image/ma.jpg" alt="" />
            <div>关注官方服务微信</div>
          </div>
          <!-- <div class="ma2">
            <img src="./image/ma.jpg" alt="" />
            <div>关注官方微信订阅号</div>
          </div> -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      big: true,
    };
  },
  mounted() {
    let w = window.screen.width;
    if (w < 1200) {
      this.big = false;
    }
  },
};
</script>

<style lang="less" scoped>
*{
  margin: 0;
  padding: 0;
}
.footer {
  height: 25vh;
  background-color: #484848;
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 100vw;
  .right {
    width: 50%;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 999;
    span {
      font-size: 12px;
      color: #fff;
      line-height: 20px;
      z-index: 999;
      
    }
  }
  .left {
    width: 50%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 100%;
    overflow: hidden;
    .img {
      width: 100%;
      height: 100%;
      margin-bottom: 2vw;
      .img1 {
        width: 40%;
      }
      .img2 {
        width: 20%;
        margin-bottom: 3.5vw;
      }
    }
  }
}
.ma {
  display: flex;
  font-size: 12px;
  color: white;
  justify-content: space-between;
  width: 20vw;
  height: auto;
  .ma1 {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: 8vw;
    text-align: center;
    height: auto;
    div{
      margin-top: 10px;
    }
  }
  .ma2 {
    display: flex;
    flex-direction: column;
    width: 8vw;
    text-align: center;
    justify-content: space-between;
  }
}
.small {
  height: 350px;
  background-color: #042423;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100vw;
  background: url(@/assets/footerBag.jpg);
  .right {
    display: flex;
    justify-content: center;
    margin-bottom: 4vh;
    span {
      font-size: 2vh;
      color: #5a5a51;
      text-align: center;
      margin-top: 50px;
      line-height: 18px;
    }
  }
  .left {
    // .ma {
    //   display: flex;
    //   font-size: 12px;
    //   color: white;
    //   justify-content: space-around;
    //   width: 100vw;
    //   .ma1 {
    //     display: flex;
    //     flex-direction: column;
    //     justify-content: space-between;
    //     width: 30vw;
    //     text-align: center;
    //     div{
    //       font-size: 1vw;

    //     }
    //   }
    //   .ma2 {
    //     display: flex;
    //     flex-direction: column;
    //     width: 40vw;
    //     text-align: center;
    //     justify-content: space-between;
    //   }
    //   div {
    //     font-size: 1vh;
    //     color: #5a5a51;
    //   }
    // }
       .ma {
      display: flex;
      font-size: 12px;
      color: white;
      justify-content: space-around;
      width: 100vw;
      .ma1 {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        width: 30vw;
        text-align: center;
        div{
          font-size: 12px;
        }
      }
      .ma2 {
        display: flex;
        flex-direction: column;
        width: 40vw;
        text-align: center;
        justify-content: space-between;
      }
      div {
        font-size: 1vh;
        color: #5a5a51;
        margin-top: 2vw;
      }
    }

  }
}
</style>