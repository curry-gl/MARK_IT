<template>
  <div class="home">
    <!-- 导航开始 -->
    <div class="nav">
      <div class="nav_content">
        <a href="#"><img src="../../public/logo1.png" alt=""><span>觅未创意</span></a>
        <a @click="show=!show" class="right" href="#"><img src="../../public/daohang.png" alt=""></a>
      </div>
    </div>
    <el-collapse-transition>
      <div class="nav_show" v-show="show">
        <div class="nav_show_content">
          <ul>
            <li><a @click="unshowHandler" href="#content2">服务介绍</a></li>
            <li><a @click="unshowHandler" href="#content_image">最新案例</a></li>
            <li><a @click="unshowHandler" href="#about">关于我们</a></li>
            <li><a @click="unshowHandler" href="#">联系我们</a></li>
          </ul>
        </div>
        </div>
      </el-collapse-transition>
    <!-- 导航结束 -->
    <!-- 主页面开始 -->
    <div class="content">
      <div class="cotent_content">
        <div class="box">
          <div class="text"><p>CRE</br> ATIV</br> ITY.</p></div>
          <div class="jiantou"><img src="../../public/daohang(1).png" alt=""></div>
        </div>
      </div>
    </div>
    <!-- 主页面结束 -->
    <!-- 主页面2开始 -->
    <div id="content2" class="content2">
      <div class="title">
        <h4 class="jieshao">服务介绍</h4>
        <div class="line"></div>
        <div class="branding">
          <div class="left">
            <img class="img1" src="../../public/2.jpg" alt="">
            <h4>咨询&设计</h4>
            <p>市场调研、产品定位、品牌核心价值提炼、品牌个性与品牌形象塑造、营销传播方案等策略内容。品牌形象、视觉识别系统（VI）设计、产品包装、销售道具、广告宣传品等设计内容。品牌／产品命名、Slogan、品牌故事、广告主题、创意脚本、活动标题、推文、软文等文案内容。</p>
          </div>
          <div class="center">
            <img class="img2" src="../../public/3.jpg" alt="">
            <h4>电商运营</h4>
            <p>我们提供一体化电商全网运营服务，包括定制与开发，全网平台运维、咨询与增值服务等。我们构建并驱动品牌电商价值。我们深耕化妆品、时尚、服装、家居、母婴、宠物等垂直类电商领域，以国际化团队为数十家国内外知名品牌提供专业高效的品牌电商服务。</p>
          </div>
          <div class="right">
            <img class="img3" src="../../public/1.jpg" alt="">
            <h4>内容营销</h4>
            <p>我们通过提供优质内容和“觅未盒子”小程序为品牌提供一站式口碑内容营销服务。深耕小红书、抖音、微博、B站、微信等社交平台。合作超过1000+优质达人和群主，涵盖时尚、美妆、健身、美食、母婴等领域。覆盖超过10000+平台用户。</p>
          </div>
        </div>
      </div>
    </div>
    <!-- 主页面2结束 -->
    <!-- 图片展示开始 -->
    <div id="content_image" class="content_image">
      <el-row :gutter="20">
        <el-col :span="8"><img src="../../public/10.jpg" alt=""></el-col>
        <el-col :span="8"><img src="../../public/9-5.jpg" alt=""></el-col>
        <el-col :span="8"><img src="../../public/8_.jpg" alt=""></el-col>
      </el-row>
      <el-row :gutter="20">
        <el-col :span="8"><img src="../../public/11.jpg" alt=""></el-col>
        <el-col :span="8"><img src="../../public/5-2.jpg" alt=""></el-col>
        <el-col :span="8"><img src="../../public/13.jpg" alt=""></el-col>
      </el-row>
      <el-row :gutter="20"> 
        <el-col :span="8"><img src="../../public/4.jpg" alt=""></el-col>
        <el-col :span="8"><img src="../../public/15-2.jpg" alt=""></el-col>
        <el-col :span="8"><img src="../../public/14-1.jpg" alt=""></el-col>
      </el-row>
      <el-row :gutter="20">
        <el-col :span="8"><img src="../../public/16.jpg" alt=""></el-col>
        <el-col :span="8"><img src="../../public/12.jpg" alt=""></el-col>
        <el-col :span="8"><img src="../../public/7.jpg" alt=""></el-col>
      </el-row>
      <el-row :gutter="20">
        <el-col :span="8"><img src="../../public/6.jpg" alt=""></el-col>
        <el-col :span="8"><img src="../../public/14.jpg" alt=""></el-col>
        <el-col :span="8"><img src="../../public/15.jpg" alt=""></el-col>
      </el-row>
    </div>
    <!-- 图片展示结束 -->
    <!-- 模态框开始 -->
    <el-dialog
      :visible.sync="dialogVisible"
      width="30%">
    </el-dialog>
    <!-- 模态框结束 -->
    <!-- 关于我们开始 -->
    <div id="about" class="about">
      <div class="about_content">
        <h4>关于我们</h4>
        <div class="line"></div>
        <div class="left">
          <h1>MEWE</h1>
          <span>IDEA.COM</span>
          <h4>觅未创意TM</h4>
          <div class="addess">
            <span>北京市朝阳区酒仙桥路14号兆维工业园C3座</span>      
            <span>电话：+86-10-80813586</span>      
            <span>邮箱：business@meweidea.com</span>      
          </div>
        </div>
        <div class="right">
          <p>我们是领先的品牌咨询&服务平台，由各领域精英组成，包括国际4A美术指导，知名设计公司设计总监、策略总监，知名互联网公司UI负责人、技术主管；</p>
          <p>我们是一支经验丰富、具有国际化视野和创新能力的团队；</p>
          <p>我们坚持“与梦想者同行”，致力于成为“从中国制造到中国创造”这场变革的重要参与者。</p>
          <img src="../../public/city.png" alt="">
        </div>
      </div>
    </div>
    <!-- 关于我们结束 -->
    <!-- 轮播图开始 -->
    <div class="carousel">
      <el-carousel :interval="4000" type="card" height="200px">
        <el-carousel-item v-for="item in photo" :key="item">
          <!-- <img :src="item.src" alt=""> -->
          <h3 class="medium">{{ item.src }}</h3>
        </el-carousel-item>
      </el-carousel>
    </div>
    <!-- 轮播图结束 -->
    <!-- 赞助开始 -->
    <div class="zanzhu">
      <div class="zanzhu_content">
          <div class="zanzhu_center">
            <img src="../../public/a1.png" alt="">
            <!-- <img src="../../public/a2.png" alt=""> -->
            <!-- <img src="../../public/a3.png" alt=""> -->
            <img src="../../public/a4.png" alt="">
            <img src="../../public/a5.png" alt="">
            <img src="../../public/a6.png" alt="">
            <img src="../../public/a7.png" alt="">
            <img src="../../public/a8.png" alt="">
            <img src="../../public/a9.png" alt="">
            <img src="../../public/a10.png" alt="">
            <img src="../../public/a11.png" alt="">
            <img src="../../public/a13.png" alt="">
          </div>
      </div>
    </div>
    <!-- 赞助结束 -->
    <!-- 脚部开始 -->
    <div class="footer">
      <div class="footer_title">
          © 2020-2025 北京觅未创意科技有限公司 版权所有 京ICP备16046633号
      </div>
    </div>
    <!-- 脚部结束 -->
    <!-- 锚点开始 -->
    <el-backtop target=".page-component__scroll .el-scrollbar__wrap"></el-backtop>
    <!-- 锚点结束 -->
  </div>
</template>

<script>
export default {
  name: 'Home',
  data(){
    return{
      show:false,
      dialogVisible:false,
      src:'',
      photo:[
        {
          src:'我徂东山，慆慆不归'
        },
        {
          src:'我来自东，零雨其濛'
        },
        {
          src:'我东曰归，我心西悲'
        }
      ]
    }
  },
  methods:{
    //点击但航隐藏
    unshowHandler(){
      this.show=false
    },
    //打开模态框显示详情
    detailsHandler(src){
      this.src=src
    }
  }
}
</script>
<style scoped>
  .zanzhu_content .zanzhu_center img{
    width: 130px;
    height: 90px;
  }
  .zanzhu .zanzhu_content .zanzhu_center{
    width: 970px;
    height: 82px;
    margin: 0 auto;
    padding-top: 98px;
  }
  .footer_title{
    width: 900px;
    height: 50px;
    margin: 0 auto;
    padding-top: 28px;
    color: #999;
    font-size: 14px;
  }
  .zanzhu_content{
    width: 100%;
    height: 411px;
  background-color: rgba(47,46,46,0.7);
  }
  .footer{
    width: 100%;
    height: 82px;
    background-color: #2f2e2e;;
  }
  .zanzhu{
    width: 100%;
    height: 411px;
    background-image: url(../../public/footer-bg.jpg);
    background-color: #fff;
    background-attachment: fixed;
    background-size: cover;
  }
  .carousel{
    width: 970px;
    height: 290px;
    margin: 0 auto;
  }
  .about_content .right img{
    width: 450px;
    height: 70px;
  }
  .about_content .right p:first-child{
    margin-top: 1px;
  }
  .about_content .right p{
    text-align: left;
    font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
    color: #333;
    font-size: 14px;
    letter-spacing: 1px;
    font-weight: bold;
  }
  .about_content .left .addess span{
    display: block;
    font-size: 14px;
    text-align: left;
    letter-spacing: 2px;
    line-height: 1.4;
  }
  .about_content .left h4{
    margin-top: 10px;
    font-size: 24px;
    font-weight: bold;
    letter-spacing: 4px;
    font-family: "Microsoft YaHei", "宋体", "Helvetica Neue",Helvetica,Arial,sans-serif;
    text-align: left;
  }
  .about_content .left span{
    font-size: 65px;
    margin: 0;
    padding: 0;
    font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
    text-align: left;
    font-weight: bold;
    line-height: 0.87;
    display: block;
    color: #333;
  }
  .about_content .left h1{
    font-size: 65px;
    margin: 0;
    padding: 0;
    font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
    text-align: left;
    line-height: 0.87;
    color: #333;
  }
  .about_content .left{
    float: left;
    width: 485px;
    height: 225px;
    margin-top: 100px;
    /* background-color: aquamarine; */
  }
  .about_content .right{
    float: right;
    width: 485px;
    height: 225px;
    margin-top: 100px;
    /* background-color: bisque; */
  }
  .about_content .line{
    width: 40px;
    height: 3px;
    margin: 0 auto;
    background-color: #f7931d;
  }
  .about_content h4{
    margin-top: 120px;
    margin-bottom: 10px;
    font-size: 22px;
    color: #2f2e2e;
    font-weight: bold;
    letter-spacing: 5px;
  }
  .about_content{
    width: 970px;
    height: 565px;
    margin: 0 auto;
  }
  .content_image{
    width: 1110px;
    margin: 0 auto;
  }
  .content_image img{
    width: 360px;
    height: 240px;
  }
  .content2 .title p{
    text-align: justify;
    margin: auto;
    font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
    font-size: 14px;
    color: #2f2e2e;
  }
  .content2 .title .branding h4{
    text-align: left;
    margin-top: 10px;
    margin-bottom: 10px;
    font-weight: 500;
  }
  .left{
    float: left;
    width: 266px;
  }
  .right{
    float: right;
    width: 266px;
  }
  .center{
    float: left;
    margin-left: 76px;
    width: 266px;
  }
  .branding img{
    width: 266px;
    height: 177px;
  }
  .nav{
    width: 100%;
    height: 60px;
    background-color: #f8f8f8;
    position: relative;
  }
  .nav_show{
    width: 100%;
    height: 60px;
    background-color: #f8f8f8;
    margin-bottom: 6px;
  }
  .nav .nav_content a{
    text-decoration: none;
    display: inline-block;
    color: #2f2e2e;
    font-size: 18px;
    font-weight: bold;
    float: left;
    letter-spacing: 5px;
  }
  .nav .nav_content a:hover{
    color: #777;
  }
  .nav .nav_content img{
    width: 28px;
    height: 28px;
    margin-top: -4px;
    display: inline;
    vertical-align: middle;
  }
  .nav_content{
    width: 970px;
    height: 60px;
    margin: 0 auto;
    /* background-color: teal; */
    line-height: 60px;
    position: relative;
  }
  .nav_show_content{
    width: 970px;
    height: 60px;
    margin: 0 auto;
    /* background-color: teal; */
    line-height: 60px;
  }
  .content2{
    width: 970px;
    height: 565px;
    margin: 0 auto;
  }
  .cotent_content{
    width: 970px;
    height: 1065px;
    margin: 0 auto;
  }
  .nav_content span{
    margin-left: 8px;
  }
  .nav .nav_content .right{
    display: inline-block;
    float: right;
  }
  .nav .nav_content .right{
    width: 28px;
    height: 19px;
  }
  .nav_show_content ul{
    list-style: none;
    float: right;
  }
  .nav_show_content ul li{
    float: left;
    margin-right: 22px;
  }
  .nav_show_content ul li:nth-child(4){
    margin-right: 5px;
  }
  .nav_show_content ul li a{
    text-decoration: none;
    color: #2f2e2e;
    font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
    font-size: 14px;
  }
  .nav_show_content ul li a:hover{
    color: #f7931d;
  }
  .content{
    width: 100%;
    height: 1065px;
    background-image: url(../../public/header-bg.jpg);
    /* background-repeat: round; */
    background-size: cover;
    background-attachment: scroll;
    margin-bottom: 120px;
  }
  .box{
    width: 360px;
    height: 465px;
    margin:300px auto;
    margin-left: 289px;
    background-color: #fff;
    position: absolute;
  }
  .text{
    text-align: center;
    color: #2f2e2e;
  }
  .text p{
    font-size: 90px;
    font-family: "Arial black", "宋体", "Helvetica Neue",Helvetica,Arial,sans-serif;
    text-align: center;
    line-height: 1;
  }
  .jiantou{
    margin-top: -52px;
  }
  .jiantou img{
    width: 61px;
    height: 55px;
  }
  /* 动画 */
  @keyframes spin {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
    transition: all 5s;
  }
}
.jiantou {
    transition: All 0.4s ease-in-out;
    -webkit-transition: All 0.4s ease-in-out;
    -moz-transition: All 0.4s ease-in-out;
    -o-transition: All 0.4s ease-in-out;
}
.jiantou:hover {
    transform: rotate(360deg);
    -webkit-transform: rotate(360deg);
    -moz-transform: rotate(360deg);
    -o-transform: rotate(360deg);
    -ms-transform: rotate(360deg);
}
.content2 .title .jieshao{
  font-size: 22px;
  color: #2f2e2e;
  font-weight: bold;
  letter-spacing: 5px;
  margin: 10px;
}
.content2 .title .line{
  width: 40px;
  height: 3px;
  margin: 0 auto;
  background-color: #f7931d;
}
.branding{
  width: 950px;
  height: 433px;
  margin: 0 auto;
  margin-top: 65px;
}
</style>
