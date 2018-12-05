<template>
  <div class='head'>
    <div class='content'>
      <a :href='tag.buttonUrl'>
        <img :src='tag.buttonImg' alt='图片不存在'>
      </a>
    </div>
    <div class='navetag'>
      <ul class='nave-li'>
        <li v-for='item of naves' :key='item.id'>
          <a :href='item.url'>{{item.value}}</a>
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      tag: {
        buttonImg: require('../assets/images/button_11.gif'),
        buttonUrl: 'http://wpa.qq.com/msgrd?v=3&uin=1326499052&site=qq&menu=yes'
      },
      naves: [
        {
          value: '首页',
          url: '',
          id: '1'
        },
        {
          value: '产品介绍',
          url: '',
          id: '2'
        },
        {
          value: '系统介绍',
          url: '',
          id: '3'
        },
        {
          value: '宫颈癌结果查询',
          url: '',
          id: '4'
        },
        {
          value: '新生儿结果查询',
          url: '',
          id: '5'
        },
        {
          value: '产前筛查结果',
          url: '',
          id: '6'
        },
        {
          value: '联系我们',
          url: '',
          id: '7'
        },
        {
          value: 'English',
          url: '',
          id: '8'
        }
      ]
    }
  }
}
</script>
<style lang='less'>
@import '../assets/less/head';
</style>
