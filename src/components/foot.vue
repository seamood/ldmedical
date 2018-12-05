<template>
  <div class='foot'>
    <div class='connect'>
      <div class='hezi bgimg'>{{name}}</div>
      <div class='hezi' v-for='item of images' :key='item.url'>
        <a :href='item.url'>
          <img :src='item.src' alt='图片不存在'>
        </a>
      </div>
    </div>
    <div class='world-tag'>
      <p>{{tag}}</p>
      <pre>{{tag2}}</pre>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      name: '相关链接',
      images: [
        {
          url: 'http://www.chinacdc.cn',
          src: require('../assets/images/zgjbyf.jpg')
        },
        {
          url: 'http://www.chinawch.org.cn',
          src: require('../assets/images/fybjzx.jpg')
        },
        {
          url: 'http://www.nhfpc.gov.cn',
          src: require('../assets/images/gjwsjsw.jpg')
        },
        {
          url: 'http://www.chinawch.com',
          src: require('../assets/images/zgfybjw.jpg')
        },
        {
          url: 'http://www.zgfywszz.com',
          src: require('../assets/images/zgfyws.jpg')
        }
      ],
      tag: '北京里定医疗网络技术服务有限公司',
      tag2: '法律声明 ICP证 黔 ICP 备 12000152 （版权所有）'
    }
  }
}
</script>
<style lang='less'>
    @import '../assets/less/foot';
</style>
