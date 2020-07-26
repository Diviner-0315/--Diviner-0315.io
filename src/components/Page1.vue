<template>
  <div class="container">
    <div class="col-md-4 col-md-offset-4 mycontent" @click.self="hideWeiXin()">
      <div class="img-circle img-content">
        <img src="../assets/img/hs.jpg" alt="" />
      </div>
      <h2 class="text-muted my-name">赵增磊</h2>
      <h3 class="my-work">
        Web前端工程师
      </h3>
      <p class="one-say">胜利永远留给有准备的人</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Page1",
  methods: {},
};
</script>

<style>
.mycontent {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.img-content {
  width: 210px;
  height: 0;
  padding-bottom: 210px;
  margin-bottom: 150px;
  border: 1px solid #aaa;
  overflow: hidden;
  transition: 1.3s;
}
.active .img-content {
  margin-bottom: 30px;
}
.img-content:hover {
  transform-origin: 50% 50%;
  animation: touPicAni ease-in-out 1.5s;
}
.img-content img {
  width: 101%;
}
.my-name {
  line-height: 1rem;
}
.my-work {
  font-weight: bold;
  line-height: 0.1rem;
  color: #f1c155;
}
.my-work em {
  font-size: 1.8rem;
  font-weight: 300;
}
.my-work a:hover {
  color: inherit;
}
.my-icon span {
  font-size: 2.2rem;
  line-height: 4rem;
  padding: 20px;
  transition-delay: 1.3s;
  transition: 1.3s;
}
.active .my-icon span {
  font-size: 2rem;
  padding: 1px;
}
.one-say {
  font-size: 2rem;
  margin-top: 10%;
  letter-spacing: 0.3em;
  text-shadow: 3px 4px 2px #aaaaaa;
  white-space: nowrap;
  color: #1482f0;
}
.popover-content img {
  width: 100%;
}

@keyframes touPicAni {
  0% {
    transform: rotateZ(0);
  }
  25% {
    transform: rotateZ(40deg);
  }
  75% {
    transform: rotateZ(-40deg);
  }
  100% {
    transform: rotateZ(0);
  }
}
  .col-md-4 .text-muted{
    color: #fff;
  }
</style>
