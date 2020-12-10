<template>
  <div>
    <div class="top">
      <div class="w header">
        <el-row class="hidden-xs-only">
          <el-col :sm="1">
            <img src="http://www.axios-js.com/logo.svg" />
          </el-col>
          <el-col :sm="1"><a href="#">文档</a></el-col>
          <el-col :sm="1"><a href="#">博客</a></el-col>
          <el-col :sm="2"><a href="#">简体中文</a></el-col>
        </el-row>
        <el-row class="hidden-sm-and-up box">
          <el-col :span="1"> 222 </el-col>
          <div>
            <img
              src="http://www.axios-js.com/logo.svg "
              height="50px"
              width="50px"
            />
          </div>
        </el-row>
      </div>
      <div class="pos">
        <div class="title">轻量级移动端Vue组件库</div>
        <div class="ins">
          <div class="install"></div>
          <div class="install_right">></div>
        </div>
      </div>
    </div>
    <div class="mid w">
      <ul class="clearfix">
        <li>
          <h2>组件</h2>
          <div>使用组件 Demo 快速体验交互细节</div>
        </li>
        <li>
          <h2>资源</h2>
          <div>
            载相关资源，用其快速搭建页面原型或高保真视觉稿，提升产品设计效率
          </div>
        </li>
        <li>
          <h2>指南</h2>
          <div>
            了解设计指南，帮助产品设计人员搭建逻辑清晰、结构合理且高效易用的产品。
          </div>
        </li>
        <li>
          <h2>主题</h2>
          <div>在线主题编辑器，可视化定制和管理站点主题、组件样式</div>
        </li>
      </ul>
    </div>
    <div class="sup">npm <span>install</span> zum/ui</div>
    <div class="start"><a href="#">开始使用</a></div>
    <footer>
      <div class="w clearfix">
        <div class="fl">
          <div>© 2020 zum/ui</div>
          <div>Documentation licensed under CC BY 4.0.</div>
        </div>
        <div class="fr"><span>1</span><span>2</span></div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {};
</script>

<style lang="less" scoped>
@import "../assets/css/varible.less";
@media screen and(max-width: 1200px) {
  .w {
    width: 100% !important;
  }
}
@media screen and(max-width: 770px) {
  .hidden-xs-only {
    display: none;
  }
  .top {
    height: 317px !important;
  }
  .title {
    width: 100% !important;
    font-size: 40px !important;
    margin-bottom: 20px !important;
  }
  .pos {
    transform: translate(-50%, -20%) !important;
  }
  .mid li {
    width: 100% !important;
  }
  .sup {
    width: 100% !important;
  }
}
.w {
  width: 1200px;
  padding: 0 20px;
  margin: 0 auto;
}

.top {
  position: relative;
  height: 535px;
  overflow: hidden;
  background-color: #171f26;
  .header {
    margin-top: 48px;
    line-height: 50px;

    & .el-col:first-child {
      width: 50px;
      height: 50px;
      img {
        width: 100%;
        height: 100%;
      }
    }
    & .el-col:nth-child(n + 1) {
      a {
        font-size: 14px;
        color: @gray_font;
        &:hover {
          color: @hv_font;
        }
      }
    }
    & .el-col:nth-child(2) {
      margin: 0 20px 0 35px;
    }
    & .el-col:nth-child(4) {
      float: right;
    }
  }
}
.pos {
  display: flex;
  flex-direction: column;
  align-items: center;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -30%);
  .title {
    width: 700px;
    text-align: center;
    font-size: 50px;
    font-weight: 300;
    margin-bottom: 45px;
    color: @gray_font;
    font-family: Lato, "Helvetica Neue", Helvetica, Arial, sans-serif;
  }
  .ins {
    display: flex;
    .install_right {
      width: 45px;
      height: 48px;
      background-color: #009688;
      line-height: 48px;
      text-align: center;
      color: #fff;
    }
  }
  .install {
    width: 228px;
    height: 47px;
    background-color: #283542;
    color: @gray_font;
    padding: 0 20px;
    line-height: 47px;
    text-align: center;
    font-size: 18px;
    &::before {
      content: "$ ";
      padding-right: 3px;
      opacity: 0.5;
    }
    &::after {
      content: "npm install zum/ui";
      font-family: Lato, "Helvetica Neue", Helvetica, Arial, sans-serif;
    }
  }
}
.box {
  position: relative;
  & div:first-child {
    color: #fff;
  }
  & div:last-child {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    color: #fff;
  }
}
.mid {
  ul li {
    float: left;
    width: 50%;
    height: 100px;
    margin: 50px 0;
    line-height: 50px;
    text-align: center;
    h2 {
      color: #009688;
    }
  }
}
.sup {
  width: 700px;
  height: 62px;
  line-height: 62px;
  padding-left: 50px;
  background-color: #eeeeee;
  margin: 0 auto;
  font-family: Lato, "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 16px;
  span {
    margin: 0 4px;
  }
  &::before {
    content: "$";
    color: #009688;
    content: "$";
    margin-right: 10px;
    font-family: Source Code Pro, "Monaco, Menlo, Consolas, monospace";
  }
}
.start {
  margin: 40px 0;
  a {
    display: block;
    width: 126px;
    height: 47px;
    margin: 0 auto;
    font: 600 15px/40px "微软雅黑";
    color: #009688;
    text-align: center;
    border: 3px solid #00dec9;
    &:hover {
      color: #fff;
      background-color: #00dec9;
    }
  }
}

footer {
  display: flex;
  align-items: center;
  color: @gray_font;
  background-color: #171f26;
  height: 122px;
  .fl {
    float: left;
  }
  .fr {
    float: right;
  }
}
</style>