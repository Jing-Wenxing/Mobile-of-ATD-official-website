<template>
  <div class="microservicetop">
    <van-notice-bar mode="link"
                    color="#2B2C30"
                    class="notice-swipe"
                    background="#ffffff"
                    @click="tomicroservice">
      微服务专区
    </van-notice-bar>

    <microservicepreview :column="false"
                         :microservicedata="this.inmicroservice_content"></microservicepreview>
  </div>
</template>

<script>
import microservicepreview from '@/components/Microservice/microservice_preview'

export default {
  components: {
    microservicepreview,
  },
  data () {
    return {
      inmicroservice_content: [
        {
          microserviceid: '10001',
          imgurl: 'https://pic.gksec.com/2020/08/10/05564be60ae6a/pexels-roberto-nickson-2762179.jpg',
          title: '微服务名称',
          subtitle: '副标题',
          activity: '233',
          description: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
          microserviceurl: 'http://jingwenxing.top/23333.mp4',
          activityitem: ['180', '35', '10', '5', '3']
        },
        {
          microserviceid: '10002',
          imgurl: 'https://pic.gksec.com/2020/08/10/05564be60ae6a/pexels-roberto-nickson-2762179.jpg',
          title: '微服务名称',
          subtitle: '副标题',
          activity: '233',
          description: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
          microserviceurl: 'http://jingwenxing.top/Marvel.mp4',
          activityitem: ['180', '35', '10', '5', '3']
        },
        {
          microserviceid: '10003',
          imgurl: 'https://pic.gksec.com/2020/08/10/05564be60ae6a/pexels-roberto-nickson-2762179.jpg',
          title: '微服务名称',
          subtitle: '副标题',
          activity: '233',
          description: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
          microserviceurl: 'http://jingwenxing.top/Marvel.mp4',
          activityitem: ['180', '35', '10', '5', '3']
        },
        // {
        //   microserviceid: '10004',
        //   imgurl: 'https://pic.gksec.com/2020/08/10/05564be60ae6a/pexels-roberto-nickson-2762179.jpg',
        //   title: '微服务名称',
        //   activity: '233',
        //   microserviceurl: 'http://jingwenxing.top/Marvel.mp4'
        // },
      ]
    };
  },
  methods: {
    tomicroservice () {
      console.log('转到微服务页')
    }
  },
}
</script>

<style>
.microservicetop {
  margin: 10px 0;
}
</style>