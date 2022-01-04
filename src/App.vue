<template>
  <div id="app">
    <MoblePage v-if="!isPC"></MoblePage>
    <PCPage v-else></PCPage>
  </div>
</template>

<script>
import MoblePage from './components/mobile/index.vue';
import PCPage from './components/pc/index.vue';
export default {
  name: 'app',
  components: {
    MoblePage,
    PCPage
  },
  data () {
    return {
      isPC: true
    }
  },
  created () {
    let mobile_bs = {
      versions: function () {
        var u = navigator.userAgent;
        return {
          trident: u.indexOf('Trident') > -1,
          presto: u.indexOf('Presto') > -1,
          webKit: u.indexOf('AppleWebKit') > -1,
          gecko: u.indexOf('Gecko') > -1 && u.indexOf('KHTML') == -1,
          mobile: !!u.match(/AppleWebKit.*Mobile.*/) || !!u.match(/AppleWebKit/) && u.indexOf(
            'QIHU') && u.indexOf('QIHU') > -1 && u.indexOf('Chrome') < 0,
          ios: !!u.match(/\(i[^;]+;( U;)? CPU.+Mac OS X/),
          android: u.indexOf('Android') > -1 || u.indexOf('Linux') > -1,
          iPhone: u.indexOf('iPhone') > -1 || u.indexOf('Mac') > -1,
          iPad: u.indexOf('iPad') > -1,
          webApp: u.indexOf('Safari') == -1
        }
      }()
    };

    if (mobile_bs.versions.mobile) {
      if (mobile_bs.versions.android || mobile_bs.versions.iPhone || mobile_bs.versions.iPad || mobile_bs.versions
        .ios) {
        this.isPC = false
      }
    };
  },
}
</script>
