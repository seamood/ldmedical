<template>
  <div class='notificationBar'>
    <div class="head">
      <p>{{tip}}</p>
    </div>
    <ul class='not-border'>
      <li v-for='item of icon' :key='item.id'>
        <div>
          <img :src='item.src' alt='图片不存在'>
        </div>
        <div>
          <p class="tip">{{item.tip}}</p>
          <p>{{item.tip2}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data () {
    return {
      tip: '服务专栏',
      icon: [
        {
          src: require('../assets/images/iphone.png'),
          id: '1',
          tip: '全国服务热线',
          tip2: '400-632-5588'
        },
        {
          src: require('../assets/images/iformation.png'),
          id: '2',
          tip: '在线咨询',
          tip2: '周一到周五8:30-18:00'
        },
        {
          src: require('../assets/images/connect.png'),
          id: '3',
          tip: '预约服务',
          tip2: '专门为您提供一对一的远程服务'
        }
      ]
    }
  }
}
</script>
<style lang="less" scoped>
 @import '../assets/less/notification';
</style>

