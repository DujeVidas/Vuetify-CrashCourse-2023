<template>
  <VApp>
    <SideBar @select-option="onSelectOption" />
    <VMain>
      <ImageGallery :isWithColor="isWithColor" />
    </VMain>
  </VApp>
</template>

<script>
import SideBar from './components/SideBar.vue'
import ImageGallery from './components/ImageGallery.vue';

export default {
  components: {
    SideBar,
    ImageGallery
  },
   data() {
    return{
      isWithColor: true
    }
   },
   methods:{
    onSelectOption(isColor){
      this.isWithColor = isColor
      console.log(this.isWithColor)

    }
   }
}
</script>