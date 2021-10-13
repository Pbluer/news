<template>
  <div class="navBar">
    <h1>sunnyside</h1>

    <nav class="menu">
      <ul>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Projects</a></li>
        <li><a href="#" id="contact">CONTACT</a></li>
      </ul>
    </nav>

    <button @click=" displayMenuMobile = !displayMenuMobile" >
      <svg width="24" height="18" xmlns="http://www.w3.org/2000/svg">
        <path
          d="M24 16v2H0v-2h24zm0-8v2H0V8h24zm0-8v2H0V0h24z"
          fill="#FFF"
          fill-rule="evenodd"
        />
      </svg>
    </button>

    <nav class="mobileMenu animate__animated animate__fadeInRight" v-if="displayMenuMobile">
      <div></div>
      <ul>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Projects</a></li>
        <li><a href="#" id="contact">CONTACT</a></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "navBar",
  props: {
    title: String,
  },
  data() {
    return {
      displayMenuMobile: false,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
.navBar {
  display: flex;
  justify-content: space-between;
  width: 80vw;
  margin: 0 auto;
  padding: 20px;

  button {
    display: none;
  }

  h1 {
    font-family: "Fraunces";
    font-weight: 900;
    font-size: 1.5rem;
    color: #fff;
  }

  ul {
    display: flex;
    list-style: none;
    justify-content: space-between;
    align-items: center;

    li {
      margin: 0 5%;

      a {
        color: #fff;
        text-decoration: none;
      }

      &:last-child {
        border-radius: 15px;
        background-color: #fff;
        padding: 10px 15px;

        &:hover {
          background-color: #3397c9;
        }
      }

      #contact {
        color: #000;
        font-weight: 700;

        &:hover {
          color: #fff;
        }
      } 
    }
  }
}

@media screen and (min-width: 375px) {
  .navBar {
    margin: 0%;
    width: 99vw;

    h1 {
      font-size: 1.5rem;
    }

    button {
      display: inherit;
      border: none;
      background-color: transparent;
      padding: auto;
      margin: auto 20px auto 0;
    }

    .menu {
      display: none;
    }

    .mobileMenu {
      position: absolute;
      background-color: #fff;
      width: 335px;
      height: 300px;      
      margin: 80px 7% auto auto;
      right: 0;

      div {
        border-radius: 100px 100px 0 0;
        height: 100px;
        width: 20px;
        background-color: #fff;
        position: absolute;
        right: 0;
        top: -20px;
      }


      ul {
        display: flex;
        flex-direction: column;
        margin: 20px;

        li {
          margin: 20px 0;

          a {
            color: rgb(99, 99, 99);
          }

          &:last-child {
            border-radius: 15px;
            background-color: #ebe413;
            padding: 10px 15px;           
          }

        }
      }
    }
  }
}
</style>
