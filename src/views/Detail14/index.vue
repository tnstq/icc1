<template>
<!-- 竞赛内容 -->
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
    <Header />
    <div :class="{ body: big, smallBody: !big }">
      <h1 style=";">Competition Rules of the 2022-2023 Invention Convention China</h1>
      <div class="top" :class="{ top2: !big }">
        <span v-if="big">作者:全球发明大会中国区</span>
        <span v-else>来源</span>
        <span class="time">发布时间: 2023-03-18</span>
        <span>39次浏览</span>
      </div>
      <div class="pdf">
        <div class="back" @click="back">< &nbsp;返回</div>
        <img src="./image/e0.jpg" alt="" />
          <img src="./image/e1.jpg" alt="" />
          <img src="./image/e2.jpg" alt="" />
          <img src="./image/e3.jpg" alt="" />
          <img src="./image/e4.jpg" alt="" />
          <img src="./image/e5.jpg" alt="" />
          <img src="./image/e6.jpg" alt="" />
          <img src="./image/e7.jpg" alt="" />
          <img src="./image/e8.jpg" alt="" />
          <img src="./image/e9.jpg" alt="" />
          <img src="./image/e10.jpg" alt="" />
          <img src="./image/e11.jpg" alt="" />
          <img src="./image/e12.jpg" alt="" />
          <img src="./image/e14.jpg" alt="" />
          <img src="./image/e15.jpg" alt="" />
          <img src="./image/e16.jpg" alt="" />
          <img src="./image/e17.jpg" alt="" />
          <img src="./image/e18.jpg" alt="" />
          <img src="./image/e19.jpg" alt="" />
      </div>
      <div :class="{ sfoot: big, smallFoot: !big }">
        <span @click="up">上一篇：无</span>
        <span @click="down"
          >下一篇：竞赛介绍 | 聚焦SDGs，15个竞赛主题蓄势待发</span
        >
      </div>
    </div>

    <Footer />
  </div>
</template>

<script>
export default {
  data() {
    return {
      big: true,
      top:false,
      y:0
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
    up() {
      
    },
    down() {
      this.$router.push({ name: "Detail13" });
    },
    back() {
      this.$router.push({ name: "News" });
    },
    handleScrollbox() {
      this.currentScroll = window.pageYOffset; //表示当前滚动的位置
      this.y = window.pageYOffset;
    },
    toTop(){
      window.scrollTo(0, 0);
    }
  },
   watch:{
    y(){
      //console.log(this.y);
      if(this.y > 150){
        this.top  = true
      }else{
        this.top = false
      }
    }
  }
};
</script>

<style lang="less" scoped>
* {
  margin: 0;
  padding: 0;
}
span,
div,
h1,
h2,
h3 {
  cursor: default;
}
.bigbox {
  display: flex;
  flex-direction: column;
  overflow-x: hidden;
  height: auto;
  .runTop{
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
    
    .icon{
      margin-top: 5px;
    }
  }
}
.body {
  h1 {

    font-size: 20px;
    color: #1c4587;
  }
  height: 120vh;
  background-color: #efefef;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  margin-top: 15vh;
  padding: 10vh 0;

//   zhangqiang
//   .top {
//     display: flex;
//     justify-content: space-around;
//     width: 100%;
//     margin-bottom: 1vh;
//     padding-bottom: 1vh;
//     font-size: 0.5vw;
//     width: 30vw;
//   }
  .top {
      display: flex;
      justify-content: center;
      width: 100%;
      margin-bottom: 1vh;
    //   padding-bottom: 1vh;
      //border-bottom: 1vh solid #d9d9d9;
      padding: 2vw 0;
      span{
        font-size: 12px;
      }
      .time {
        margin: 0 3vh;
      }
    }
  .pdf {
    height: 100%;
    width: 50%;
    background-color: #fff;
    overflow: scroll;
    border-top: 2px solid #9a9a9a;
        border-left: 2px solid #9a9a9a;
    img {
      width: 100%;
    }
  }
}
.smallBody {
  height: 100vh;
  width: 100vw;
  h1 {
    // margin-bottom: 3vh;
    font-size: 2vw;
    display: block;
       font-family:SimSun;
       font-size:18px;
       color:#426100;
       font-weight:bold;
       text-decoration:none;
       text-align:center;
       line-height: 30px
  }
  .top {
    display: flex;
    justify-content: center;
    width: 100%;
    margin-bottom: 1vh;
    padding-bottom: 1vh;
    border-bottom: 1vh solid #d9d9d9;
    padding: 2vw 0;
    span {
      display: inline-block;
      font-size: 14px;
      opacity: 0.7;
    }
    .time {
      margin: 0 3vh;
    }
  }
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  padding: 8vh 0;
  .pdf {
    height: 100%;
    width: 100%;
    background-color: #fff;
    overflow: scroll;

    img {
      width: 100%;
    }
  }
}
.sfoot {
  display: flex;
  flex-direction: column;
  margin-left: -30%;
  margin-top: 2vw;
  font-family: SimSun;
  font-size: 12px;
  color: #444 !important;
  font-weight: normal;
  line-height: 25px;
  span:hover {
    color: skyblue;
  }
}
.smallFoot {
    width: 100%;
  font-size: 12px;
  display: flex;
  flex-direction: column;
  margin: 5vh 0;
  span{
    width: 90%;
    padding: 1vh 0;
        overflow: hidden; // 文字超长隐藏
    text-overflow:ellipsis; // 显示...
    white-space: nowrap; // 单行显示
  }
}

// zhangqiang
// .back {
//   padding: 10px;
//   font: 15px Arial, "宋体", Helvetica, sans-serif, Verdana;
// }
.back{
  padding: 10px;
  font-size: 13px;
  font-weight: bold;
//   font: 15px Arial,"宋体",Helvetica, sans-serif,Verdana;
}
.back:hover {
  color: skyblue;
}
</style>