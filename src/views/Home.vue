<template>
  <div class="home">
    <h2 class="title">一个弹幕视频demo</h2>
    <d-player :options="options">
    </d-player>
  </div>
</template>

<script>
// @ is an alias to /src
import VueDPlayer from 'vue-dplayer'
import 'vue-dplayer/dist/vue-dplayer.css'


export default {
  data() {
    return {
      options: {
        video: {
          url: './voide/9979161.mp4',
          // pic: '//i2.hdslb.com/bfs/archive/b76a7e12f4696757fc8f48f7f781cb85e61e4da4.jpg@560w_350h_100Q_1c.webp'
        },
        autoplay: false,
        danmaku: {
            id: '4157142',
            api: 'http://127.0.0.1:1207/',
            token: 'tokendemo',
            user: 'TuGe7025',
            bottom: '15%',
            unlimited: true,
        }
      }
    }
  },
  components: {
    'd-player':VueDPlayer
  }
}
</script>
