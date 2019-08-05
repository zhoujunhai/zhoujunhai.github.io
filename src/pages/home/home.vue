<template>
  <div id="top"
       class="home">
    <top>
      <vue-particles color="#ffffff"
                     :particleOpacity="0.7"
                     linesColor="#ffffff"
                     :particlesNumber="80"
                     shapeType="circle"
                     :particleSize="5"
                     :linesWidth="2"
                     :lineLinked="true"
                     :lineOpacity="0.4"
                     :linesDistance="2"
                     :moveSpeed="3"
                     :hoverEffect="true"
                     hoverMode="grab"
                     :clickEffect="true"
                     clickMode="push">
      </vue-particles>
    </top>
    <div class="menu"
         id="menu"
         v-show="menuFixed">
      <ul>
        <li class="nav">
          <a href="#top">首页</a>
        </li>
        <li class="nav">
          <a href="#about">关于我</a>
        </li>
        <li class="nav">
          <a href="#experience">经历</a>
        </li>
        <li class="nav">
          <a href="#skill">技能</a>
        </li>
        <li class="nav">
          <a href="#bottom">联系我</a>
        </li>
      </ul>
    </div>
    <div id="about">
      <about></about>
    </div>
    <div id="experience">
      <experience />
    </div>
    <div id="skill">
      <skill />
    </div>
    <div id="bottom">
      <bottom />
    </div>
  </div>
</template>

<script>
import top from '@/components/top'
import bottom from '@/components/bottom'
import about from '@/components/about'
import experience from '@/components/experience'
import skill from '@/components/skill'
import project from '@/components/project'
export default {
  name: 'home',
  data () {
    return {
      menuFixed: false
    }
  },
  components: {
    top,
    bottom,
    about,
    experience,
    skill,
    project
  },
  mounted () {
    window.addEventListener('scroll', this.handleScroll)
    window.addEventListener('beforeunload', this.handleBeforeunload)
  },
  methods: {
    handleScroll () {
      let scrollTop = window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop
      this.menuFixed = scrollTop > 650
    },
    handleBeforeunload () {
      console.log("test111111111111")
      // this.$router.push({ name: "Home" })
      this.$route.query.redirect || '/'
    },
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.home {
  min-width: 1200px;
  height: auto;
}
.menu {
  display: block;
  text-align: center;
  width: 100%;
  position: fixed;
  left: 0px;
  top: 0px;
  background: #ffffff;
}
.nav {
  display: inline-block;
  font-size: 19px;
  font-family: "Microsoft YaHei", sans-serif;
  padding: 20px;
}
a {
  text-decoration: none;
  color: #000;
}
a:hover {
  color: #ef7674;
}
</style>

