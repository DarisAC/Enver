<template>
    <footer class="footer">
        <MainContainer>
            <div class="footer__contant">
                <div class="logo">
                    <img src="../assets/image/logo.png" alt="" class="logo_icon">
                    <p class="logo_text">Enver</p>
                </div>
                <div class="footer-nav">
                    <div class="nav_item" v-for="(menu, index) in footerNavList" :key="index">
                        <router-link :to="menu.path">
                        {{ menu.name }}
                        </router-link>
                    </div>
                </div>
                <div class="footer-copyright">© 2020 Enver, All Rights Reserved</div>
            </div>
        </MainContainer>   
    </footer>
</template>

<script>
import MainContainer from '@/components/MainContainer.vue';


export default {
  name: 'Home',
  components: {
    MainContainer
  },
  data() {
    return {
      footerNavList: [
        { name: 'Supports', path: '/'},
        { name: 'Privacy Policy', path: '/'},
        { name: 'Terms and Conditions', path: '/'},
     
      ]
    }
  }
}
</script>