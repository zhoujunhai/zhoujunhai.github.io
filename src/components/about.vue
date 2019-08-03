<template>
  <div class="about">
    <div class="container">
      <span class="tip">WHO AM I</span>
      <h1 class="title">{{title}}</h1>
      <span class="border one"></span>
      <div class="a_info">
        <ul>
          <li>
            <p>较强的团队意识，在工作中能与同事之间相互协助、友好交流，更高效的完成工作。</p>
          </li>
          <li>
            <p>较好的表达能力与沟通能力；工作积极主动，能尽心尽责地完成本职工作，具备较强的学习与创新能力。</p>
          </li>
          <li>
            <p>求知欲旺盛，对事物有较强的分析能力，敢于接受新的挑战。</p>
          </li>
          <li>
            <p>热爱程序员工作，有敬业精神，做事专注，抗压力强，工作态度严谨、细心。</p>
          </li>
          <li>
            <p>具有多年的银行业务开发经验，对银行业务有深刻的理解，特别是四川人行支付结算系统和ETC系统，负责建行四川省分行同城清算业务一期和二期业务的主要建设和运维工作，熟悉普通贷记往来账、实时贷记往来账、实时借记往来账、定期借贷记往来账、公用事业扣款协议、非公用事业扣款协议、小额快速扣款协议和个人扣款协议等业务流程和其他辅助交易业务流程，熟悉人行接口文档及整个清算系统业务。</p>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import 'swiper/dist/css/swiper.css'
import { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  name: 'about',
  data () {
    return {
      title: '自我简述',
      swiperOption: {
        spaceBetween: 30,
        centeredSlides: true,
        autoplay: {
          delay: 2500,
          disableOnInteraction: false
        },
        pagination: {
          el: '.swiper-pagination',
          clickable: true
        },
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev'
        }
      }
    }
  },
  components: {
    swiper,
    swiperSlide
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.about {
  height: auto;
  width: 100%;
  margin: 0 auto;
  background-color: #f5f5f5;
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
.a_info {
  width: 60%;
  margin: 0 auto;
}
.a_info ul {
  margin-top: 10px;
  border-top: 1px solid #fff;
  text-align: left;
}
.a_info ul li {
  font-size: 20px;
  margin-top: 26px;
}
.swiper-container {
  width: 100%;
  height: 300px;
  line-height: 300px;
  overflow: hidden;
  text-align: center;
}
.swiper-pagination {
  top: 46%;
}
</style>
