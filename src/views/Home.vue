<template>
  <section class="our-services">
    <MainContainer>
        <div class="our-services__presentation">
          <div class="our-services__content">
            <h1>Build Your Awesome Platform</h1>
            <p>Enver studio is a digital studio that offers several services such as UI/UX Design to developers, we will provide the best service for those of you who use our services.</p>
            <button class="button">Our revices
               <img src="../assets/image/arrow.png" alt="">
            </button>
          </div>
          <div class="our-services__image" >
            <div v-for="(imageList,index) in ourServicesImageList" :key="index">
               <img :src="require(`@/assets/image/${imageList.image}`)" :class="imageList.class" />

            </div>
            <!-- <img src="../assets/image/z.png" alt="" class="img-z">
            <img src="../assets/image/our-services_back.png" alt="" class="img-our-services_back">
            <img src="../assets/image/our-services_main.png" alt="" class="img-our-services_main">
            <img src="../assets/image/circles.png" alt="" class="img-circles">
            <img src="../assets/image/play.png" alt="" class="img-play">
            <img src="../assets/image/add.png" alt="" class="img-add"> -->
          </div>   
        </div>
    </MainContainer>
  </section>
  <section class="why-enver">
    <MainContainer>
      <div class="why-enver__presentation">
        <div class="why-enver__content">
          <h1 class="why-enver_title">
            Why Enver Is The Best Choice?
          </h1>
          <p class="why-enver_text">
            Watch this one minute video so you understand why you should use our services!
          </p>
        </div>
        <div class="why-enver__video">
          <img src="../assets/image/video.png" alt="">
          <img src="../assets/image/playVideo.png" alt="" class="video-button">
        </div>
      </div>
    </MainContainer>
  </section>
</template>

<script>
// @ is an alias to /src
import MainContainer from '@/components/MainContainer.vue';


export default {
  name: 'Home',
  components: {
    MainContainer
  },
  data(){
    return {
      ourServicesImageList:[
        { image: "z.png" , class: "img-z" },
        { image:"our-services_back.png", class: "img-our-services_back" },
        { image:"our-services_main.png", class: "img-our-services_main" },
        { image: "circles.png", class: "img-circles" },
        { image: "play.png", class: "img-play" },
        { image: "add.png", class: "img-add" }
      
    ]
    
  }
  
}}
</script>

<style lang="scss" scoped>
.why-enver{
  margin-top: 150px;
  .why-enver__content{
    display: flex;
    justify-content: space-between;
    .why-enver_title{
      max-width: 390px;
    }
    .why-enver_text{
      font-size: 14px;
      max-width: 390px;
      font-weight: normal;
    }
  }
  .why-enver__video{
    margin-top: 30px;
    position: relative;
    .video-button{
      position: absolute;
      top: 50%;
      left: 50%;
      margin-right: -50%;
      transform: translate(-50%, -50%)
    }
  }
}
</style>