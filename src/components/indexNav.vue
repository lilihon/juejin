<template>
  <div class="outside-container">
    <div class="inside-container">
      <span class="up-navitem"><img class="logo" src="https://lf3-cdn-tos.bytescm.com/obj/static/xitu_juejin_web/e08da34488b114bd4c665ba2fa520a31.svg" alt="logo" ></span>
      <span class="up-navitem"><a href="#">首页</a></span>
      <span class="up-navitem"><a href="#">沸点</a></span>
      <span class="up-navitem"><a href="#">课程</a></span>
      <span class="up-navitem"><a href="#">直播</a></span>
      <span class="up-navitem"><a href="#">活动</a></span>
      <span class="up-navitem"><a href="#">竞赛</a></span>
      <span class="up-navitem"><a href="#">商城</a></span>
      <span class="up-navitem"><a href="#">APP</a></span>
      <span class="up-navitem"><a href="#">插件</a></span>
      <span class="up-navitem"><a href="#"><img class="report" src="https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/0cb52d4a506e44aba88bc0f2e8a8b2b7~tplv-k3u1fbpfcp-zoom-1.image" alt=""></a></span>
      <span class="up-navitem">
        <span class="serc"></span>
          <input type="text" placeholder="搜索稀土掘金" name="search">
          <button class="ser" type="submit"><img src="https://lf3-cdn-tos.bytescm.com/obj/static/xitu_juejin_web/1e8ab9a22f0ddc36349f60b38900d0bd.svg" alt=""></button>
      </span>
      <span class="up-navitem develop"><a href="#"><button>创作者中心<i class="more fa fa-angle-down"></i></button></a></span>
      <span class="up-navitem"><a href="#">会员</a><img class="img-vip" src="https://lf3-cdn-tos.bytescm.com/obj/static/xitu_juejin_web/24127194d5b158d7eaf8f09a256c5d01.svg" alt=""></span>
      <span class="up-navitem">
      <button @click="1" class="register"><a href="#">登录</a><i>|</i><a href="#">注册</a></button>
      </span>
    </div>
  </div>
  <div class="nav-list">
    <div class="nav-cont">
    <span class="nav-item" :class="tabKey === 'zonghe' ? 'active' : ''" @click="handleChangeTab('zonghe')">综合</span>
    <span class="nav-item" :class="tabKey === 'houduan' ? 'active' : ''" @click="handleChangeTab('houduan')">后端</span>
    <span class="nav-item" :class="tabKey === 'frontd' ? 'active' : ''" @click="handleChangeTab('frontd')">前端</span>
    <span class="nav-item" :class="tabKey === '1' ? 'active' : ''" @click="handleChangeTab('1')">Android</span>
    <span class="nav-item" :class="tabKey === 'ios' ? 'active' : ''" @click="handleChangeTab('ios')">iOS</span>
    <span class="nav-item" :class="tabKey === '3' ? 'active' : ''" @click="handleChangeTab('3')">人工智能</span>
    <span class="nav-item" :class="tabKey === '4' ? 'active' : ''" @click="handleChangeTab('4')">开发工具</span>
    <span class="nav-item" :class="tabKey === '5' ? 'active' : ''" @click="handleChangeTab('5')">代码人生</span>
    <span class="nav-item" :class="tabKey === '6' ? 'active' : ''" @click="handleChangeTab('6')">阅读</span>
    </div>
  </div>
  <div>
    <Zonghe v-if="tabKey ==='zonghe'"/>
    <Frontd v-if="tabKey === 'frontd'" />
    <IOS v-if="tabKey === 'ios'" />
  </div>
  <div class="right-blo">
    <Right/>
  </div>
</template>

<script>
import Frontd from './frontd.vue'
import IOS from './ios.vue'
import Zonghe from './zonghe.vue'
import Right from './right.vue'
export default {
  name: 'IndexNav',
  components: {
    Frontd,
    IOS,
    Zonghe,
    Right
  },
  data() {
    return {
      tabKey: 'zonghe'
    }
  },
  methods: {
    handleChangeTab(value) {
      console.log(value);
      this.tabKey = value
    },
    handleRegister(){
      console.log('登录');
    }
  }
}
</script>
<style>
.outside-container{
    background: white;
    border-bottom: 1px solid #f1f1f1;
    color: #909090;
    /* height: 5rem; */
    z-index: 250;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    transition: all .2s;
    font-family: sans-serif;
}
.inside-container{
    height: 50px;
    max-width: 1440px;
    align-items: center;
    line-height: 1;
    margin: 0 auto;
    position: relative;

}
.up-navitem{
    display: flex;
    float: left;
    color: #86909c;
    padding: 0 0.9rem;
    font-size: 0.95rem;
    padding: auto;
    height: 100%;
    justify-content: center; 
    align-items: center;
    cursor: pointer; 
    top: 20px;
}

input{
  height: 24px;
  border-radius: 2px;
  align-items: center;
  border: 2px solid #71777c;
  /* margin-bottom: 3px; */
}
.ser{
  position: relative;
    left: -2px;
    width: 35px;
    height: 30px;
    border-radius: 2px;
    align-content: center;
    border: 1px solid #71777c;
}
.up-navitem a{
  text-decoration:none;
  color: #86909c;
  /* align-items: center; */
}
.up-navitem a:hover{
  color: #007fff;
}
.logo{
    /* display: block; */
    width: 107px;
    height: 20px;
    border-style: none;


}
.report{
    max-width: 115px;
    vertical-align: middle;
    border-style: none;
}

.develop{
  width: 115px;
  height: 35px;
  padding: 0 1rem;
  font-size: 1.167rem;
  white-space: nowrap;
  
}
.develop button{

    height: 38px;
    color: white;
    background-color: #007fff;
    border-radius: 3px;
    border: #007fff;
    margin-top: 5px;
}

.register{
  background: rgba(30,128,255,.05);
    border: 1px solid rgba(30,128,255,.3);
    border-radius: 4px;
    padding: 0.1rem 1rem;
    color: #007fff;
    line-height: 1.5rem;
    font-size: 14px;
    font-weight: 400;
    margin-right: 2rem;
    height: 3rem;
}
.register i{
  padding: 0 4px;
}
.img-vip{
    width: 24px;
    height: 24px;
}
.nav-list {
  /* position: fixed; */
  left: 0;
  top: 0;
  width: 100%;
  box-shadow: 0 1px 2px 0 rgb(0 0 0 / 5%);

}
.nav-list .nav-cont{
  height: 35px;
  max-width: 960px; 
  display: flex;
  align-items: center;
  line-height: 1;
  margin: 0 auto;
}
.nav-list .nav-item {
  font-size: 0.85rem;
  color: #71777c;
  text-decoration: none;
  padding: 0 1rem;
  cursor: pointer;
}
.nav-list .nav-item.active{
  color: rgb(108, 155, 224);
}
.right-blo{
  float: right;
  margin-right: 200px;
}
</style>