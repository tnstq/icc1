<template>
  <div class="bigbox">
    <div v-if="top" :class="{ runTop: top }" @click="toTop">
      <svg
        t="1678766219182"
        class="icon"
        viewBox="0 0 1024 1024"
        version="1.1"
        xmlns="http://www.w3.org/2000/svg"
        p-id="3026"
        width="18"
        height="18"
      >
        <path
          d="M512 378.24l-418.88 418.88L0 704l512-512 512 512-93.12 93.12z"
          fill="#fff"
          p-id="3027"
        ></path>
      </svg>
    </div>
    <Header></Header>
    <div v-if="big" class="body">
      <h1 class="hOne">2022-2023年度全球发明大会中国区参赛材料</h1>
      <span class="text"
        >参赛团队需完成一项原创发明项目，并准备发明原型或模型、发明日志、发明展板和路演视频。</span
      >
      <!-- 四个动画图片 -->
      <div class="an">
        <div class="one">
          <div class="top"></div>
          <div class="img">
            <img src="./image/1.png" alt="" />
          </div>
          <div class="foot">
            <span>发明日志</span>
            <!-- 下面的小字 -->
            <span class="footerText">记录你的发明故事</span>
          </div>
        </div>
        <div class="one">
          <div class="top"></div>
          <div class="img">
            <img src="./image/2.png" alt="" />
          </div>
          <div class="foot">
            <span>发明展板</span>
            <!-- 下面的小字 -->
            <span class="footerText">展示你的发明故事</span>
          </div>
        </div>
        <div class="one">
          <div class="top"></div>
          <div class="img">
            <img src="./image/3.png" alt="" />
          </div>
          <div class="foot">
            <span>路演视频</span>
            <!-- 下面的小字 -->
            <span class="footerText">讲述你的发明故事</span>
          </div>
        </div>
        <div class="one">
          <div class="top"></div>
          <div class="img">
            <img src="./image/4.png" alt="" />
          </div>
          <div class="foot">
            <span>发明原型</span>
            <!-- 下面的小字 -->
            <span class="footerText">呈现你的发明故事</span>
          </div>
        </div>
      </div>
      <!-- 下面的 pdf -->
      <div class="pdf">
        <div class="top">
          <img src="./image/5.png" alt="" class="img1" />
          <img src="./image/6.png" alt="" class="img2" />
          发明日志参考模板
        </div>
        <strong>本发明日志仅作为参考模板，并非唯一标准。</strong>
        <span>
          你可发挥创意，自行设计更有趣的、带有自身特色的发明日志，但内容须包括发明过程的记录。</span
        >
        <!-- 放pdf图片 -->
       <div class="pdfContainer">
          <!-- 放第一个pdf图片 -->
          <div class="pdfImg1">
            <img src="./image/a0.jpg" alt="" />
            <img src="./image/a1.jpg" alt="" />
            <img src="./image/a2.jpg" alt="" />
            <img src="./image/a3.jpg" alt="" />
            <img src="./image/a4.jpg" alt="" />
            <img src="./image/a5.jpg" alt="" />
            <img src="./image/a6.jpg" alt="" />
            <img src="./image/a7.jpg" alt="" />
            <img src="./image/a8.jpg" alt="" />
            <img src="./image/a9.jpg" alt="" />
            <img src="./image/a10.jpg" alt="" />
            <img src="./image/a11.jpg" alt="" />
            <img src="./image/a12.jpg" alt="" />
            <img src="./image/a13.jpg" alt="" />
            <img src="./image/a14.jpg" alt="" />
            <img src="./image/a15.jpg" alt="" />
            <img src="./image/a16.jpg" alt="" />
            <img src="./image/a17.jpg" alt="" />
            <img src="./image/a18.jpg" alt="" />
            <img src="./image/a19.jpg" alt="" />
            <img src="./image/a20.jpg" alt="" />
            <img src="./image/a21.jpg" alt="" />
            <img src="./image/a22.jpg" alt="" />
          </div>
          <!-- 放第二个pdf图片 -->
          <div class="pdfImg2">
            <img src="./image/0.jpg" alt="" />
            <img src="./image/1.jpg" alt="" />
            <img src="./image/2.jpg" alt="" />
            <img src="./image/3.jpg" alt="" />
            <img src="./image/4.jpg" alt="" />
            <img src="./image/5.jpg" alt="" />
            <img src="./image/6.jpg" alt="" />
            <img src="./image/7.jpg" alt="" />
            <img src="./image/8.jpg" alt="" />
            <img src="./image/9.jpg" alt="" />
            <img src="./image/10.jpg" alt="" />
            <img src="./image/11.jpg" alt="" />
            <img src="./image/12.jpg" alt="" />
            <img src="./image/13.jpg" alt="" />
            <img src="./image/14.jpg" alt="" />
            <img src="./image/15.jpg" alt="" />
            <img src="./image/16.jpg" alt="" />
            <img src="./image/17.jpg" alt="" />
            <img src="./image/18.jpg" alt="" />
            <img src="./image/19.jpg" alt="" />
            <img src="./image/20.jpg" alt="" />
          </div>
        </div>
      </div>
    </div>
    <!-- 移动端 -->
    <div v-else class="pmd-outer">
      <!-- 标题 -->
      <h1 class="hOne">2022-2023区竞赛材料</h1>
      <div class="hOne-line"></div>
      <span class="pmd-sidehead"
        >参赛团队需完成一项原创发明项目，并准备发明原型或模型、发明日志、发明展板和路演视频。</span
      >
      <!-- 四个卡片区块 -->
      <div class="pmd-cards">
        <!-- 第一块 -->
            <div class="pmd-cardsOne" >
                <span><img class="cardsImg" src="./image/1.png" alt=""></span>
                <span>发明日志</span>
                <span class="pmd-cardsOne-lastText">记录你的发明故事</span>  
            </div>

            <!-- 第2块 -->
            <div class="pmd-cardsOne" >
                <span><img class="cardsImg" src="./image/2.png" alt=""></span>
                <span>发明展板</span>
                <span class="pmd-cardsOne-lastText">展示你的发明故事</span>  
            </div>

            <!-- 第3块 -->
            <div class="pmd-cardsOne" >
                <span><img class="cardsImg" src="./image/3.png" alt=""></span>
                <span>路演视屏</span>
                <span class="pmd-cardsOne-lastText">讲述你的发明故事</span>  
            </div>

            <!-- 第4块 -->
            <div class="pmd-cardsOne" >
                <span><img class="cardsImg" src="./image/4.png" alt=""></span>
                <span>发明原型</span>
                <span class="pmd-cardsOne-lastText">呈现你的发明作品</span>  
            </div>
      </div>

      <!-- 线 -->
      <div class="hOne-line"></div>
      <!--  -->
      <div class="topT">
            发明日志参考模板
            <img src="./image/5.png" alt="" class="img1" />
            <img src="./image/6.png" alt="" class="img2" />
          </div>

      <div class="pmd-showContent">
        <span>※该页面手机端无法完整显示</span>
        <span>请前往PC端官方网站进行浏览</span>
      </div>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      big: true,
      top: false,
      y: 0,
    };
  },
  mounted() {
    window.addEventListener("scroll", this.handleScrollbox, true);
    window.scrollTo(0, 0);
    let w = window.screen.width;
    if (w < 1200) {
      this.big = false;
    }
  },
  methods: {
    handleScrollbox() {
      //this.currentScroll = window.pageYOffset; //表示当前滚动的位置
      this.y = window.pageYOffset;
    },
    toTop() {
      window.scrollTo(0, 0);
    },
  },
  watch: {
    y() {
      //console.log(this.y);
      if (this.y > 150) {
        this.top = true;
      } else {
        this.top = false;
      }
    },
  },
};
</script>

<style lang="less" scoped>
* {
  margin: 0;
  padding: 0;
}
span,div,h1,h2,h3{
  cursor: default;
}
.bigbox {
  overflow-x: hidden;
  .runTop {
    position: fixed;
    right: 10px;
    bottom: 20vh;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    background-color: #1d1d1d;
    z-index: 1000;
    text-align: center;
    margin: 0 auto;
    color: #fff;

    .icon {
      margin-top: 5px;
    }
  }
}
.body {
  width: 100%;
  margin-top: 15vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  .hOne {
    width: 60%;
    border-bottom: 2px solid #ff5a00;
    height: 10vh;
    margin: 0 auto;
    font-size: 24px;
    text-align: center;
    line-height: 10vh;
    animation: an 1s 5 alternate;
  }
  .text {
    display: inline-block;
    width: 60%;
    height: 20vh;
    margin: 0 auto;
    text-align: center;
    line-height: 20vh;
    font-size: 14px;
  }
  /* 四个动画 */
  .an {
    width: 60%;
    display: flex;
    justify-content: space-between;
    .one {
      width: 20%;
      height: 25vh;
      background-color: #f5f5f5;
      display: flex;
      flex-direction: column;
      align-items: center;
      animation: rotateZ 1s;
      .top {
        width: 2vw;
        height: 2vh;
        border-top: 2px solid #ff9900;
      }
      .img {
        width: 5vw;
        height: 5vw;
        img {
          width: 5vw;
          height: 5vw;
          text-align: center;
        }
      }
      .foot {
        width: 10vw;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
        span {
          text-align: center;
          font-size: 14px;
        }
        .footerText {
          font-family: 微软雅黑;
          font-size: 12px;
          margin-top: 5vh;
        }
      }
    }
  }
  .pdf {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 10vh;
    /* 发明日志参考模板 */
    .top {
      width: 250px;
      height: 60px;
      position: relative;
      text-align: center;
      line-height: 60px;
      font-size: 24px;
      font-weight: 700;
      margin-bottom: 5vh;
      /* 左上小三角 */
      .img1 {
        position: absolute;
        left: 0;
        top: 0;
      }
      /* 右下小三角 */
      .img2 {
        position: absolute;
        right: 0;
        bottom: 0;
      }
    }
    strong {
      font: 12px/140% Arial, "宋体", Helvetica, sans-serif, Verdana;
      color: #5a5a5a;
      font-weight: 900;
      font-size: 14px;
    }
    span {
      font-size: 14px;
      margin-bottom: 10vh;
    }
    .pdfContainer {
      display: flex;
      justify-content: space-around;
      width: 80vw;
      margin-bottom: 100px;
      .pdfImg1 {
        //background-color: red;
        height: 100vh;
        width: 35vw;
        display: flex;
        flex-direction: column;
        overflow: scroll;
        border-top: 2px solid #9a9a9a;
        border-left: 2px solid #9a9a9a;
        img {
          width: 100%;
        }
      }
      .pdfImg2 {
        //background-color: red;
        height: 100vh;
        width: 35vw;
        display: flex;
        flex-direction: column;
        overflow: scroll;
        border-top: 2px solid #9a9a9a;
        border-left: 2px solid #9a9a9a;
        img {
          width: 100%;
        }
      }
    }
  }
}
/* 标题下的线条动画 */
@keyframes an {
  from {
    width: 40%;
  }
  to {
    width: 60%;
  }
}
/* 旋转动画 */
@keyframes rotateZ {
  from {
    transform: rotateY(-180deg);
  }
  to {
    transform: rotateY(0);
  }
}

// 移动端的样式
.pmd-outer {
  padding: 0 14px;
  // 标题行
  .hOne {
    font-size: 19px;
    text-align: center;
    margin: 30px 0 20px 0;
  }
  // 分割线
  .hOne-line {
    width: 100%;
    height: 2.5px;
    margin: 20px auto;
    background: #ff5a00;
    // opacity: 0.9;
  }

//   
  .topT {
        position: relative;
        width: 100%;
        height: 20px;
        font-weight: 700;
        font-size: 20px;
        text-align: center;
        line-height: 20px;
        color: #5a5a5a;
        margin-top: 40px;
        .img1 {
          position: absolute;
          left: 20px;
          top: -10px;
        }
        .img2 {
          position: absolute;
          right: 20px;
          bottom: -10px;
        }
      }

  // 内容
  .pmd-showContent {
    margin: 40px 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 3px;
    span {
      font-size: 18px;
      font-family: "微软雅黑";
      color: #5a5a5a;
    }
  }

    //副标题
    .pmd-sidehead {
    font-size: 16px;
    font-family: "微软雅黑";
    text-align: justify;
    color: #5a5a5a;
  }

//   卡片区块样式
.pmd-cards{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    
    // 每一块卡片的设置
    .pmd-cardsOne{
        width: 200px;
        height: 200px;
        margin: 20px 0;
        background: #f5f5f5;
        display: flex;
        flex-direction: column;
        gap: 10px;
        align-items: center;
        justify-content: center;
      animation: rotateZ 2s;


        // 里面图标的设置
        .cardsImg{
            width: 80px;
            height: 80px;
        }

        span{
            font-size: 16px;
            font-family: "微软雅黑";
        }
        // 第三行文字的设置
        .pmd-cardsOne-lastText{
            font-size: 14px;
            color: #5a5a5a;
        }
    }
}
}
</style>