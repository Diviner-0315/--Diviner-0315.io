<template>
  <div class="container">
    <div class="col-md-4 col-md-offset-4 mycontent">
      <h1 class="page-title">工作经历</h1>
      <div class="teach-block my-ani">
        <span class="leader-icon"></span>
        <h2 class="work-title">
          山东方大工程有限公司 <span class="text-muted">Web前端开发工程师</span>
        </h2>
        <p class="teach-time ">2018.03 - 至今</p>
        <ul class="work-detail">
          <li>负责相关产品的需求以及前端程序的实现，提供合理的前端架构；</li>
          <li>与产品、后台开发人员保持良好沟通。</li>
          <li>按照需求独立完成各种特效制作负责相关产品的需求以及前端程序的实现，提供合理的前端架构</li>
          <li>负责页面通过标准检验，兼容各个主流浏览器</li>
          <li>优化产品界面，为用户提供更好的体验 </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page3",
};
</script>

<style scoped>
h1,
h2,
h3,
p {
  margin: 2px;
}
.leader-icon {
  width: 35px;
  height: 35px;
  border: 5px solid #6ca6cd;
  border-radius: 50%;
  position: absolute;
  left: -60px;
  top: 0px;
}
.leader-icon::before {
  content: "";
  width: 7px;
  height: 7px;
  border-radius: 50%;
  background: #333333;
  position: absolute;
  top: 9px;
  left: 9px;
}
.leader-icon::after {
  content: "";
  width: 5px;
  height: 330%;
  background: #333333;
  position: absolute;
  top: 40px;
  left: 10px;
}
.leader2::after {
  height: 350%;
}
.my-ani {
  position: relative;
  left: 60px;
  width: 100%;
  margin-top: 80px;
  margin-left: 0;
}
.active .my-ani {
  margin: 3px;
}
.work-title span {
  font-size: 20px;
}
.work-detail {
  font-size: 15px;
  margin-left: 30px;
}
</style>
