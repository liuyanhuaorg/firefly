<template>
  <div class="f-card" :style="'margin:'+margin+';padding:'+padding+';'">
    <slot name="card-content"></slot>
  </div>  
</template>

<script>
export default {
  props:{
    margin:{
      type: String,
      default:'0px 0px'
    },
    padding: {
      type: String,
      default: '0px 0px'
    }
  }
}
</script>

<style lang="stylus" scoped>
@require '../stylus/color.styl'
.f-card
  background: $secondarycolor.gray
  border-radius: 5px
  -moz-box-shadow:2px 2px 20px $primarycolor.gray
  -webkit-box-shadow:2px 2px 20px $primarycolor.gray
  box-shadow:2px 2px 20px $primarycolor.gray
</style>
