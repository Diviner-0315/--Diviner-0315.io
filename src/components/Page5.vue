<template>
    <div class="container">
        <div class="col-md-4 col-md-offset-4 mycontent">
            <h1 class="page-title">工作经历</h1>
            <div class="teach-block my-ani">
                <span class="leader-icon"></span>
                <h2 class="work-title">
                    杭州口岸国际物流有限公司 <span class="text-muted">Web前端实习生</span>
                </h2>
                <p class="teach-time ">2018.07 - 2019.06</p>
                <ul class="work-detail">
                    <li>负责公司微信小程序页面的制作</li>
                    <li>实现各种页面特效与交互效果</li>
                    <li>数据交互和网页美化</li>
                    <li>优化用户体验</li>
                </ul>
            </div>
            <div class="learn-class my-ani">
                <span class="leader-icon"></span>
                <h2 class="work-title">
                    温州网纳网络科技有限公司 <span class="text-muted">Web前端工程师</span>
                </h2>
                <p class="teach-time ">2019.07 - 至今</p>
                <ul class="work-detail">
                    <li>负责公司产品的前端页面制作</li>
                    <li>优化代码兼容性</li>
                    <li>优化产品界面，为用户提供更好体验</li>
                    <li>数据交互以及各种功能的调试</li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Page5",
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
