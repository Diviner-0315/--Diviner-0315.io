<template>
  <div class="container">
    <div class="col-md-4 col-md-offset-4 mycontent">
      <h1 class="page-title">教育背景</h1>
      <div class="teach-block my-ani">
        <p class="teach-time text-center">2012.09 - 2016.06</p>
        <h2 class="text-center">潍坊科技学院 本科</h2>
        <h3 class="text-center">计算机科学与技术专业</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page2",
};
</script>

<style>
h1,
h2,
h3,
h4,
p {
  font-family: "楷体", "宋体", "微软雅黑";
  white-space: nowrap;
}
@keyframes title-ani {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.2);
  }
  100% {
    transform: scale(1);
  }
}
.text-center {
  text-align: center;
  margin: 2px;
}
.page-title {
  transition-delay: 0.2s;
  transition: 1s;
  font-size: 50px;
  font-weight: bold;
  padding-bottom: 300px;
  color: #ffff;
}
.active .page-title {
  padding-bottom: 40px;
  animation: title-ani ease 1.3s;
}
.teach-time {
  font-size: 15px;
}
.learn-class {
  margin: 30px 0;
}
.my-ani {
  opacity: 0;
  transition: 1.3s;
  margin-left: 150px;
}
.active .teach-block {
  transition-delay: 0.5s;
  opacity: 1;
  margin: 0;
}
.active .learn-class {
  transition-delay: 1s;
  opacity: 1;
  margin: 30px 0;
}
.active .get-reward {
  transition-delay: 1.5s;
  opacity: 1;
  margin: 0;
}
</style>
