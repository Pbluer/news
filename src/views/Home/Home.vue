<template>
  <div class="home">
    <header>
      <NavBar/>
      
      <div class="textCenter">
        <h1>WE ARE CREATIVES</h1>
        <img src="../../assets/images/icon-arrow-down.svg" alt="arrow" >      
      </div>
    </header>

    <Main/>
    <Cliente />
    <Galery />
    <BaseFooter />
  </div>
</template>

<script>

import NavBar from '@/components/Navbar.vue'
import Main from './Main.vue'
import Cliente from './Cliente.vue'
import Galery from './Galery.vue'
import BaseFooter from '@/components/BaseFooter.vue'


export default {
  name: 'Home',
  data() {
    return {      
    }
  },
  components: {
    NavBar,
    Main,
    Cliente,
    Galery,
    BaseFooter
  }
}
</script>

<style lang="less" scoped>
  .home {
    height: 100vh;
    background-image: url('../../assets/images/desktop/image-header.jpg');
    background-repeat: no-repeat;
    background-size: 100%;

    header {
      height: 100%;
    }
    
    .textCenter{
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      align-items: center;
      height: 60%;
      padding-top: 80px;

      h1 {
        font-family: 'Fraunces';
        font-weight: 900;
        font-size: 2.5rem;
        color: #fff;
        letter-spacing: 5px;
      }

    }

  }

  @media screen and ( min-width: 375px ) {

    .home{
      background-image: url('../../assets/images/mobile/image-header.jpg');

      header {
        height: 138vw;
      }
      
      .textCenter{
        padding-top: 20px;
        height: 48%;

        h1 {
         text-align: center;
       }

      }

    }
    
  }

</style>