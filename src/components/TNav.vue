<template>
<x-header :left-options="{showBack: showBack, backText: ''}" :style="{'background-color':bgcolor}">
  <span :style="{'color': textcolor}">{{title}}</span>
</x-header>
</template>

<script>
  import { XHeader } from 'vux/src/components/'
  export default {
    components: {
      XHeader
    },
    props: {
      // 导航栏颜色
      bgcolor: {
        type: String,
        default: '#f5f5f5'
      },
      textcolor: {
        type: String,
        default: '#333'
      },
      title: String,
      showBack: {
        type: Boolean,
        default: true
      }
    }
  }
</script>

<style scoped>

</style>
