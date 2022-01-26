<template>
    <section class="modal-window">
        <MainContainer>
            <div class="modal-window__presentation">
                <div class="modal-window_contant">
                    <div class="modal-window_close"><img src="../assets/image/close.png" alt="" class="modal-window_img" @click="showModalWindow"></div>
                    
                    <img src="../assets/image/video.png" alt="" class="modal-window_video"></div>
                
            </div>
            
        </MainContainer>   
    </section>
</template>

<script>
import MainContainer from '@/components/MainContainer.vue';


export default {
  name: 'Home',
  components: {
    MainContainer

    },
    data(){
    return {
      isShowModalWidnow: true
    }},
    methods: {
   showModalWindow() {
     this.isShowModalWidnow = false
   } 
  }
  }
</script>
<style lang="scss" scoped>

.modal-window{
    margin-top: -160px;
    position: fixed;
    z-index: 1;
    background: rgba(105,105,105, 0.7);
    height: 100%;
    width: 100%;
    &__presentation{
        position: absolute;
      top: 50%;
      left: 50%;
      margin-right: -50%;
      transform: translate(-50%, -50%);
      
    }
    &_close{
        position: relative;
    }
    &_img{
          position: absolute;
      top: 25px;
      right: 25px;
     
      max-width: 25px;
      max-height: 25px;

    }
}
</style>