<template>
    <div class="zonghe_cont">
    <div class="small_nav">
        <span class="item">推荐</span>
        <span class="item">热榜</span>
        <span class="item">最新</span>
    </div>
  <div>
<Tuijian></Tuijian>
<Rebang></Rebang>
<Zuixin></Zuixin>
  </div>
</div>
</template>

<script>
import Tuijian from './tuijian.vue'
import Rebang from './rebang.vue'
import Zuixin from './zuixin.vue'
export default {
name:'Zonghe',
components:{
    Tuijian,
    Rebang,
    Zuixin
}
}
</script>

<style>
.zonghe_cont{
    max-width: 660px;
    margin: 0 auto;
}
.small_nav .item:hover{
    color: #007fff;
}
.small_nav .item{
    color: #909090;
    cursor: pointer;
    padding: 5px 15px;
}
.small_nav{
    display: flex;
    justify-content: center;
}
</style>