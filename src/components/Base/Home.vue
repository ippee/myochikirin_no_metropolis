<template>
  <div class="home" ref="home">
    <h1>ホーム</h1>

    <div class="titles" ref="titles">
      <ul>
        <li class="title" v-for="shortStory in ShortStories" :key="shortStory.title">
          <a @click="toContent(shortStory.index)">{{ shortStory.title }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import AppRef from '@/mixins/AppRef'
import SaveData from '@/mixins/SaveData'
import ShortStories from '@/mixins/ShortStories'

export default {
  name: 'home',
  props: { index: Object },
  computed: {
    AppRef() {
      return AppRef
    },
    SaveData() {
      return SaveData
    },
    ShortStories() {
      return ShortStories
    },
  },
  mounted: function() {
    this.$refs.home.classList.add('fadein')
  },
  methods: {
    toContent: function(idx) {
      this.$refs.titles.style.pointerEvents = 'none'

      this.index.i = Number(idx)

      window.__TAURI__.tauri.invoke({
        cmd: 'playSE',
        file_name: 'bell',
        volume: SaveData.methods.getSEVol()
      })
      
      let appRef = AppRef.methods.getRef()
      appRef.classList.add('fadeout-long')
      setTimeout(function() {
        this.$router.push('/content')
      }.bind(this), 3000)
    }
  }
}
</script>

<style>
.title {
  margin-bottom: 1.2rem;
}
</style>