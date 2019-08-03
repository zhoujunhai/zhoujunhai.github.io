<template>
  <div class="experience">
    <div class="container">
      <span class="tip">WHERE I DID</span>
      <h1 class="title">{{title}}</h1>
      <span class="border"></span>
      <ul class="content">
        <li>
          <div class="content_left tx_right">
            <span class="s1"></span>
            <h4>2007.09 - 2011.07 </h4>
          </div>
          <div class="content_right tx_left">
            <h4>电子科技大学成都学院</h4>
            <p>专业：信息与计算科学</p>
          </div>
          <div class="clearfix"></div>
        </li>
        <li>
          <div class="content_left tx_right">
            <span class="s2"></span>
            <h4>2011.07 - 2012.01 </h4>
          </div>
          <div class="content_right tx_left">
            <h4>高伟达软件股份有限公司</h4>
            <p>成都农商银行二代支付项目</p>
          </div>
          <div class="clearfix"></div>
        </li>
        <li>
          <div class="content_left tx_right">
            <span class="s1"></span>
            <h4>2012.01 - 2013.12 </h4>
          </div>
          <div class="content_right tx_left">
            <h4>高伟达软件股份有限公司</h4>
            <p>对建行甘肃分行特色业务系统开发及维护（包括柜面、网银等渠道代中间业务系统、公积金系统、柜面交易系统等开发维护工作及惠普unix系统32位机器想64位机器迁移等工作）</p>
          </div>
          <div class="clearfix"></div>
        </li>
        <li>
          <div class="content_left tx_right">
            <span class="s2"></span>
            <h4>2014.01 - 现&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在 </h4>
          </div>
          <div class="content_right tx_left">
            <h4>高伟达软件股份有限公司</h4>
            <p>对建行四川分行各应用系统的开发和维护，担任项目经理，业务包括ETC系统、四川人行支付结算系统一期及二期、各州市招投标系统、省市及地市州社保系统代发代扣、pos清算系统、维修金系统、特色前台、金融知识库系统、督办系统、新一代员工渠道等的需求分析、开发测试、上线及上线后运维工作</p>
          </div>
          <div class="clearfix"></div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'experience',
  data () {
    return {
      title: '学历与工作'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.experience {
  height: auto;
  width: 100%;
  margin: 0 auto;
  background-color: #fff;
  text-align: center;
}
.container {
  height: auto;
  max-width: 1200px;
  margin: 0 auto;
  padding: 4% 0;
}
.tip {
  display: inline-block;
  position: relative;
  padding: 6px 20px;
  margin: 0 auto 10px;
  font-size: 20px;
  background: #ef7674;
  color: #fff;
}
.tip:after {
  position: absolute;
  width: 0;
  height: 0;
  left: 42%;
  bottom: -10px;
  content: "";
  border-style: solid;
  border-width: 10px 10px 0 10px;
  border-color: #ef7674 transparent;
}
.title {
  padding: 6px 0 10px;
  font-family: "Overlock", cursive;
  color: #2f2c06;
  font-size: 36px;
}
.border {
  display: block;
  width: 20%;
  height: 1px;
  position: relative;
  margin: 0 auto 30px;
  background: #8c8989;
}
.border:after {
  position: absolute;
  top: 0;
  left: 30%;
  content: " ";
  width: 40%;
  height: 5px;
  margin-top: -2px;
  background: #ef7674;
}

ul.content {
  padding-top: 20px;
}
ul.content li {
  font-size: 20px;
  color: #999;
  position: relative;
}
.content_left {
  width: 50%;
  float: left;
  padding: 25px 6% 0 0;
}
.content_left h4 {
  display: inline-block;
  position: relative;
  padding: 10px 40px;
  font-size: 20px;
  color: #fff;
  background-color: #1b242f;
}
/* 绝对定位居中，如果在没有固定高度宽度的盒子里，不要使用百分比定位，使用px，rem，居中用50%+margin负值 */
.content_left h4:before {
  width: 0;
  height: 0;
  position: absolute;
  top: 50%;
  margin-top: -6px;
  right: -10px;
  content: "";
  border-style: solid;
  border-width: 6px 0 6px 10px;
  border-color: transparent transparent transparent #1b242f;
}
.content_right {
  width: 50%;
  float: left;
  padding: 20px 0 10px 6%;
}
.content_right h4 {
  display: inline-block;
  padding: 10px 50px;
  margin-bottom: 6px;
  font-size: 20px;
  border: 1px solid #d4d4d4;
  color: #1b242f;
  box-shadow: 0 1px 6px rgba(0, 0, 0, 0.175);
}
.content_right p {
  line-height: 20px;
  font-size: 14px;
}
/*小图标*/
ul.content li span {
  position: absolute;
  top: 30px;
  right: -19px;
  z-index: 10;
  width: 36px;
  height: 36px;
  border-radius: 50%;
  background: url("../common/images/icon.png") no-repeat center;
  background-size: 50%;
}
ul.content li .s1 {
  background-color: #44c7f4;
}
ul.content li .s2 {
  background-color: #eb5424;
}

.tx_left {
  position: relative;
  text-align: left;
  box-sizing: border-box;
  border-left: 1px solid #999;
}
.tx_right {
  position: relative;
  text-align: right;
  box-sizing: border-box;
}
</style>
