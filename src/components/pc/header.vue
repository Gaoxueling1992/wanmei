<template>
  <div class="header">
    <a href="javascript:void(0)" onclick="openUrl();" rel="nofollow" style="margin-right:1%;"><img id="logo" src="./images/logs.png"
            alt="完美体育"></a>
    <h1 class="title_word">
      <a href="javascript:void(0)" onclick="openUrl();" rel="nofollow"
          class="disNone">永久网址:<font color="red">www.20wm.com</font></a>
      <a href="javascript:void(0)" onclick="openUrl();"
          rel="nofollow">永久网址:<font color="red">www.20wm.com</font></a>
    </h1>
    <a href="javascript:void(0)" onclick="openUrl()" rel="nofollow" class="btn">进入官网</a>
    <a style="width: 1.2rem;" href="javascript:void(0)" onclick="downloadApp();" rel="nofollow"
        class="btn">开始疯狂</a>
  </div>
</template>
<script>
export default {
  name: 'Header'
}
</script>
<style>
.header {
  height: 1.2rem;
  -webkit-box-shadow: 0 0 0.25rem #e7eaea;
  box-shadow: 0 0 0.25rem #e7eaea;
  padding: 0 2.5rem;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 99999;
  background: #fff;
}

.header #logo {
  width: 2.8rem;
  padding-top: 8%;
}

.header h1.title_word a {
  color: #2a2a2a;
  font-size: 0.54rem;
  font-weight: bold;
  word-break: break-all;
  white-space: nowrap;
  -webkit-animation: fadeIn 1000ms both;
  animation: fadeIn 1000ms both;
}

.header a.btn {
  margin-left: 10px;
  width: 1.6rem;
  height: 0.4rem;
  border-radius: 0.05rem;
  text-align: center;
  line-height: 0.4rem;
  color: white;
  font-size: 0.2rem;
  -webkit-animation: pulse 1000ms infinite both;
  animation: pulse 1000ms infinite both;
  /* Safari 5.1 - 6.0 */
  background: -webkit-gradient(linear, left top, left bottom, from(#00aeff), to(#1f94cb));
  background: -o-linear-gradient(#00aeff, #1f94cb);
  background: linear-gradient(#00aeff, #1f94cb);
  /* 标准的语法 */
}

.header a.btn:hover {
  -webkit-box-shadow: 0 0.03rem 0.08rem rgba(28, 151, 209, 0.69);
  box-shadow: 0 0.03rem 0.08rem rgba(28, 151, 209, 0.69);
  -webkit-animation: normal;
  animation: normal;
}
</style>
