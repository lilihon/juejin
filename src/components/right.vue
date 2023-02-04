<template>
  <div class="index-aside aside">
    <div class="signin-tip signin">
      <div class="frist-line">
        <div class="icon-text">
            <span class="title">限时领取掘金会员</span>
            <div class="second-line">点亮在社区的每一天</div>
        </div>
        <div class="sign-in-with-animation">
          <img src="https://lf3-cdn-tos.bytescm.com/obj/static/xitu_juejin_web/img/sign.d62085a.gif" alt="去签到">
        </div>
      </div>
      <div class="sidebar-block banner-block">
        <div class="banner banner">
          <a href="https://juejin.cn/post/7185104994801025061?utm_source=web1&utm_medium=banner&utm_campaign=tlgt2023">
            <img class="banner-image" src="https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/3183037b25b74c12a3843a00c7e2c09e~tplv-k3u1fbpfcp-no-mark:480:400:0:0.awebp?" alt="">
          </a>
          <div class="crtl-box">
            <i class="icon-close-round close-btn"></i>
            <a class="lable" href="https://bd.juejin.cn/?utm_campaign=bd&utm_source=web&utm_medium=banner/"></a>
          </div>
        </div>
      </div>
      <div class="sidebar-block app-download-sidebar-block sider-block shadow">
        <div class="block-body">
          <a href="/app">
            <div class="app-link">
              <img class="qr-img" src="https://lf3-cdn-tos.bytescm.com/obj/static/xitu_juejin_web/img/home.59780ae.png" alt="">
              <div class="content-box">
                <div class="headline">下载稀土掘金APP</div>
                <div class="desc">一个帮助开发者成长的社区</div>
              </div>
            </div>
          </a>
        </div>
      </div>
      <div class="sidebar-block user-block">
        <div class="recommend-author-block sticky-author-block">
          <header class="user-block-header">🎖️作者榜</header>
          <div class="user-list">
            <div class="item">
              <a href="https://juejin.cn/user/2634854380340008">
                <img src="https://p3-passport.byteimg.com/img/user-avatar/b9a366997037d998063135bd56302b85~100x100.awebp" class="lazy avatar avatar" alt="京东云开发者的头像">
                <div class="user-info">
                  <a href="https://juejin.cn/user/2634854380340008" class="username username">
                    <span class="name" style="max-width: 128px;">京东云开发者</span>
                    <span class="rank">
                      <img src="//lf3-cdn-tos.bytescm.com/obj/static/xitu_juejin_web/img/lv-5.d08789d.png" alt="">
                    </span>
                  </a>
                </div>
              </a>
            </div>
            <div class="item">
              <a href="https://juejin.cn/user/3702810893364350">
                <img src="https://p3-passport.byteimg.com/img/user-avatar/b9a366997037d998063135bd56302b85~100x100.awebp" class="lazy avatar avatar" alt="京东云开发者的头像">
                <div class="user-info">
                  <a href="https://juejin.cn/user/2634854380340008" class="username username">
                    <span class="name" style="max-width: 128px;">京东云开发者</span>
                    <span class="rank">
                      <img src="//lf3-cdn-tos.bytescm.com/obj/static/xitu_juejin_web/img/lv-5.d08789d.png" alt="">
                    </span>
                  </a>
                </div>
              </a>
            </div>
            <div class="item">
              <a href="https://juejin.cn/user/430664288573789">
                <img src="https://p3-passport.byteimg.com/img/user-avatar/b9a366997037d998063135bd56302b85~100x100.awebp" class="lazy avatar avatar" alt="京东云开发者的头像">
                <div class="user-info">
                  <a href="https://juejin.cn/user/2634854380340008" class="username username">
                    <span class="name" style="max-width: 128px;">京东云开发者</span>
                    <span class="rank">
                      <img src="//lf3-cdn-tos.bytescm.com/obj/static/xitu_juejin_web/img/lv-5.d08789d.png" alt="">
                    </span>
                  </a>
                </div>
              </a>
            </div>
            <a href="https://juejin.cn/recommendation/authors/recommended"></a>
          </div>
        </div>
      </div>
  </div>

</div>
<!-- <div class="big">
  mo
</div> -->
</template>

<script>
export default {
  name: 'Right',
};
</script>

<style>
.aside{
  width: 240px;
  overflow: hidden;
}
.signin-tip{
  padding: 16px;
  background-color: aliceblue;
  box-sizing: border-box;
}
.frist-line{
    flex-direction: row;
    align-items: center;
    justify-content: space-between;

}
.sign-in-with-animation{
  width: 74px;
  height: 36px;
  cursor: pointer;
}
.sign-in-with-animation img {
    overflow: clip;
    width: 60px;
    float: right;
}
.banner-image{
  width: 210px;
}
.qr-img{
  width: 30px;
}
a{
  text-decoration: none;
  color: #000;
}
.app-link{
  display: flex;
}
.headline{

}
.lazy.avatar{
  display: flex;
  flex: 0 0 auto;
    width: 3.8rem;
    height: 3.8rem;
    border-radius: 50%;
    margin-right: 0.5rem;

}
.user-block-header{
  display: flex;
}
.name{

}
/* .big{
  background-color: brown;
  height: 200px;
  width: 240px;
} */
/* .aside{
    position: absolute;
    top: 0;
    right: 0;
    width: 240px;
    height: 500px;
    background-color: #1d2129;

}
.index-aside{
  width: 20rem;
    position: absolute;
    top: 0;
    right: 0;
    z-index: 1;
}
.index-aside .signin{
    width: 240px;
    margin-bottom: 16px;
}
.signin-tip{
  padding: 16px;
    background-color: #fff;
    box-sizing: border-box;
}
.first-line{
  display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}
.first-line .icon-text{
  display: flex;
    flex-direction: column;
}
.first-line .title
{
  color: #1d2129;
    font-size: 16px;
    font-weight: 600;
    line-height: 24px;
}
.second-line{
  color: #8a919f;
    font-size: 12px;
    font-weight: 400;
    line-height: 24px;
}
.sign-in-with-animation{
  width: 74px;
    height: 36px;
    cursor: pointer;
}
img{
  border-style: none;
}

.sidebar-block.banner-block{
  overflow: hidden;
}
.sidebar-block.banner-block .banner{
    height: 200px;
}
.sidebar-block.banner-block .banner{
    height: 200px;
}
a{
  
    text-decoration: none;
    cursor: pointer;
    color: #909090;
}
.banner .banner-image{
    width: 100%;
    height: 100%;
}


.banner {
    position: relative;
    font-size: 0;
    cursor: pointer;
}


.banner .ctrl-box .close-btn{
    position: absolute;
    top: 0.5rem;
    right: 0.5rem;
    font-size: 1rem;
    color: #909090;
    opacity: .5;
    display: none;
}
.banner .ctrl-box .close-btn {
    position: absolute;
    top: 0.5rem;
    right: 0.5rem;
    font-size: 1rem;
    color: #909090;
    opacity: .5;
    display: none;
}
.banner .ctrl-box .label{
    position: absolute;
    right: 10px;
    bottom: 10px;
    line-height: 36px;
    height: 36px;
    font-size: 20px;
    z-index: 1;
    transform: scale(.5);
    -webkit-transform: scale(.5);
    transform-origin: right bottom;
    -webkit-transform-origin: right bottom;
    color: #fff;
    background-color: rgba(0,0,0,.2);
    border: 1px solid #fff;
    border-radius: 6px;
    padding-left: 15px;
    padding-right: 15px;
    font-weight: 300;
}
.sidebar-block {
    background-color: #fff;
  }

    .sidebar-block[data-v-71f2d09e] {
    position: relative;
    margin-bottom: 1.5rem;
    border-radius: 2px;
    }
    .sidebar-block {
    position: relative;
    margin-bottom: 1.5rem;
    border-radius: 2px;
    }
    .headline {
    font-weight: 500;
    font-size: 14px;
    line-height: 22px;
    color: #1d2129;
}
.desc{
    margin-top: 0.5rem;
    font-size: 12px;
    line-height: 20px;
    color: #86909c;
}
.sidebar-block.sticky-block{
    position: fixed;
    background-color: transparent;
    box-shadow: none;
    opacity: 0;
    transition: all .2s;
    width: 20rem;
    z-index: -1;
    top: 67px;
    pointer-events: none;
}
.recommend-author-block {
    background-color: #fff;
}
.recommend-author-block .user-block-header {
    padding: 1rem 1.3rem;
    border-bottom: 1px solid hsla(0,0%,59.2%,.1);
}
.recommend-author-block .item .link {
    padding: 1rem 1.3rem;
    display: flex;
    align-items: center;
    cursor: pointer;
}
.recommend-author-block .item .link .avatar {
    flex: 0 0 auto;
    width: 3.8rem;
    height: 3.8rem;
    border-radius: 50%;
    margin-right: 0.5rem;
}
.avatar{
    display: inline-block;
    position: relative;
    background-position: 50%;
    background-size: cover;
    background-repeat: no-repeat;
}
.recommend-author-block .item .link .username[data-v-edec7d04] {
    font-size: 1.16rem;
    font-weight: 400;
    color: #333;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    margin-bottom: 3px;
}

.recommend-author-block .item .link .username {
    font-size: 1.16rem;
    font-weight: 400;
    color: #333;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    margin-bottom: 3px;
}
.username{
  
    font-size: 1.25rem;
    font-weight: 600;
    color: var(--juejin-font-1);
    display: flex;
    align-items: center;

}

element.style {
    max-width: 128px;
}
.recommend-author-block .username .name{
    max-width: 130px;
}
.username .name[data-v-0ef8bafa] {
    display: inline-block;
    vertical-align: top;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
}
.rank {
    display: inline-flex;
    align-items: center;
    margin-left: 0.33rem;
    vertical-align: middle;
}
.rank img[data-v-3de16c56] {
    width: 35px;
    height: 16px;
} */
</style>