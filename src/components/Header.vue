<template>
    <nav class="header">
      <MainContainer>
        <div class="header__contant">
          <div class="logo">
            <img src="../assets/image/logo.png" alt="" class="logo_icon">
            <p class="logo_text">Enver</p>
          </div>
          <div class="header-nav">
            <div class="nav_item" v-for="(menu, index) in headerNavList" :key="index">
              <router-link :to="menu.path" aria-current="page" class="nav_itemsssss">
                 {{ menu.name }}
              </router-link>
            </div>
          </div>
          <div class="header__button">
            <button class="button">Contact us</button>
          </div>
        </div>
      </MainContainer>
    </nav>
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
      headerNavList: [
        { name: 'Home', path: '/'},
        { name: 'Services', path: '/services'},
        { name: 'Our project', path: '/our_project'},
        { name: 'About us', path: '/about_us'}
      ]
    }
  }
}
</script>
