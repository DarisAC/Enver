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
          <div class="our-services__image">
            <img src="../assets/image/z.png" alt="" class="img-z">
            <img src="../assets/image/our-services_back.png" alt="" class="img-our-services_back">
            <img src="../assets/image/our-services_main.png" alt="" class="img-our-services_main">
            <img src="../assets/image/circles.png" alt="" class="img-circles">
            <img src="../assets/image/play.png" alt="" class="img-play">
            <img src="../assets/image/add.png" alt="" class="img-add">
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
  }
}
</script>
