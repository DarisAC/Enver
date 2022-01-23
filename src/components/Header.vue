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
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      headerNavList: [
        { name: 'Home', path: '/'},
        { name: 'Services', path: '/Services'},
        { name: 'Our project', path: '/Our project'},
        { name: 'About us', path: '/About us'}
      ]
    }
  }
}
</script>
