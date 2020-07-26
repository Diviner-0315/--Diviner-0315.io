<template>
  <div class="container">
    <div class="col-md-6 col-md-offset-3 mycontent">
      <h1 class="page-title">专业技能</h1>
      <div class="my-container" v-for="(item, index) in skills" :key="index">
        <div class="col-xs-4 skill-content">
          <p class="text-muted skills">{{ item.name }}</p>
        </div>
        <div class="col-xs-8">
          <div class="progress progress-content">
            <div
              :class="[
                'progress-bar',
                'progress-bar-info',
                'pro-default',
                'pro' + index,
              ]"
            >
              <p class="progress-text">{{ item.pro }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import $ from "jquery";
export default {
  name: "Page4",
  data() {
    return {
      skills: [
        {
          name: "HTML",
          pro: "80%",
        },
        {
          name: "JavaScript",
          pro: "80%",
        },
        {
          name: "css/css3",
          pro: "80%",
        },
        {
          name: "Jquery",
          pro: "75%",
        },
        {
          name: "Bootstrap",
          pro: "70%",
        },
        {
          name: "Ajax",
          pro: "65%",
        },
        {
          name: "Vue",
          pro: "65%",
        },
      ],
      getProText: "",
    };
  },
  mounted: function() {
    $.each($(".progress-text"), function(i, value) {
      let tempNum = parseInt(value.innerText);
      if (tempNum > 75) {
        $(".progress-text")
          .eq(i)
          .addClass("progress-bar-info")
          .text("擅长");
      } else if (tempNum > 50) {
        $(".progress-text")
          .eq(i)
          .addClass("progress-bar-success")
          .text("熟悉");
      } else {
        $(".progress-text")
          .eq(i)
          .addClass("progress-bar-warning")
          .text("了解");
      }
    });
  },
};
</script>

<style>
.my-container {
  width: 95%;
}
.skills {
  font-size: 20px;
  line-height: 20px;
  text-align: center;
}
.progress-text {
  font-size: 1.5rem;
}
.progress-content {
  box-shadow: 0 0 4px 1px #d4d4d4;
}
.pro-default {
  transition: 2.3s ease-out;
  width: 0;
}
.active .pro0,
.active .pro1,
.active .pro2 {
  width: 80%;
}
.active .pro3 {
  width: 75%;
}
.active .pro4 {
  width: 70%;
}
.active .pro5 {
  width: 65%;
}
.active .pro6 {
  width: 65%;
}
.active .pro7 {
  width: 25%;
}
.active .pro8 {
  width: 20%;
}
@media screen and (max-height: 990px) {
  .skill-content {
    margin: -5px;
  }
}
 .my-container .text-muted{
    color: #4AB7BD;
  }
</style>
