<template>
  <transition name="el-zoom-in-bottom">
    <el-card class="box-card" v-show="show" shadow="hover">
      <div slot="header" class="clearfix">
        <span id="title">时间轨迹</span>
      </div>
      <div class="block">
        <el-timeline>
          <el-timeline-item timestamp="2019/5/9" placement="top">
            <el-card class="card" shadow="hover">
              <h2>demo 1.5</h2>
              <p>提交github</p>
              <a href="https://github.com/1045462757/55mm" target="_Blank">55mm</a>
              <p>tiga 提交于 2019年5月9日15:01:18</p>
            </el-card>
          </el-timeline-item>

          <el-timeline-item timestamp="2019/4/30" placement="top">
            <el-card class="card" shadow="hover">
              <h2>demo 1.4</h2>
              <p>界面样式再次优化</p>
              <p>tiga 提交于 2019年4月30日23:45:08</p>
            </el-card>
          </el-timeline-item>

          <el-timeline-item timestamp="2019/4/27" placement="top">
            <el-card class="card" shadow="hover">
              <h2>demo 1.3</h2>
              <p>界面样式优化</p>
              <p>tiga 提交于 2019年4月27日20:59:20</p>
            </el-card>
          </el-timeline-item>

          <el-timeline-item timestamp="2019/4/22" placement="top">
            <el-card class="card" shadow="hover">
              <h2>demo 1.2</h2>
              <p>
                1.本项目目前只涉及到前端，后端服务尚在开发，所以目前该项目的所有数据都是假的（^_^）
                <br>2.本网站所涉及的数据来自
                <a href="http://www.shehuishe.com/" target="_Blank">摄会社 - 摄影师模特摄影约拍平台</a>
                <br>3.前端基于vue 2.0 element-ui ...
              </p>
              <p>tiga 提交于 2019年4月22日19:18:17</p>
            </el-card>
          </el-timeline-item>

          <el-timeline-item timestamp="2019/4/19" placement="top">
            <el-card class="card" shadow="hover">
              <h2>demo 1.1</h2>
              <p>
                整体框架搭建， 实现了一些
                <span id="tip">简陋</span>的功能,还有很多坑需要踩
              </p>
              <p>tiga 提交于 2019年4月19日19:36:17</p>
            </el-card>
          </el-timeline-item>

          <el-timeline-item timestamp="2019/4/13" placement="top">
            <el-card class="card" shadow="hover">
              <h2>demo 1.0</h2>
              <p>tiga 提交于 2019年4月13日17:31:02</p>
            </el-card>
          </el-timeline-item>
        </el-timeline>
      </div>
    </el-card>
  </transition>
</template>

<script scoped>
export default {
  name: "About",
  data() {
    return {
      show: false
    };
  },
  methods: {},
  mounted() {
    this.show = true;
    this.$refs.cropper.startCrop();
  }
};
</script>

<style scoped>
.box-card {
  width: 95%;
  margin: 20px auto;
  border-radius: 10px;
  max-width: 1200px;
}
.clearfix {
  font-size: 20px;
}

.block {
  width: 95%;
  margin: 0 auto;
}

.card {
  margin-top: 20px;
}
.card:hover {
  background: #c8cfd4;
}
#tip {
  color: brown;
}
p {
  font-size: 18px;
  /* font-size: 1rem; */
}
a:hover {
  color: brown;
  text-decoration: underline;
}
#title {
  font-size: 24px;
  font-weight: bold;
  letter-spacing: 5px;
}
</style>
